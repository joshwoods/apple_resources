

- VisionKit
-  Enabling Live Text interactions with images 

Article

# Enabling Live Text interactions with images

Add a Live Text interface that enables users to perform actions with text and QR codes that appear in images.

## Overview

Enhance the user experience with images in your app by adding standard Live Text interactions. Live Text lets users tap text in an image to copy it, make a call, send an email, translate it, or look up directions. VisionKit provides this familiar Live Text interface to your images and across platforms.

For iOS apps, users can use a long-press gesture (touch and hold) a QR code to follow a link or take another action, depending on the payload. The payload is the data that a QR code contains, such as a URL or email address.

Before interacting with items in an image, the user can tap the Live Text button in the lower-right corner to highlight the recognized items. Then a data-specific action menu appears when the user double-taps on text in an image, and uses a long-press gesture on an email address or QR code.

In your app, you decide whether Live Text recognizes text and data within text, and for iOS apps, QR codes in the image. You choose the types of items to look for and run the analysis on the image, and then VisionKit provides the entire Live Text interface with the breadth of actions for specific types.

Important

The code listings in this article use asynchronous methods that you invoke from an `async` method or within a Task structure. For details on asynchronous flows, see Concurrency.

### Check whether the device supports Live Text

Before showing a Live Text interface in your app, check whether the device supports Live Text. For iOS apps, the image analyzer is available only on devices with the A12 Bionic chip and later. If the `ImageAnalyzer` isSupported property is `true`, show the Live Text interface. Otherwise, disable any feature in your app that relies on Live Text. If you attempt to start the Live Text interface when this property is `false`, the interface doesn’t appear.

### Add a Live Text interaction object to your view in iOS

For iOS apps, you add the Live Text interface by adding an interaction object to the view containing the image. If you use a UIImageView to display the image, it handles the image content area calculations for you.

Add an ImageAnalysisInteraction object directly on the view containing the image.

```
let interaction = ImageAnalysisInteraction()
imageView.addInteraction(interaction)
```

Optionally, customize the interface by setting the interaction’s delegate to an object that implements the ImageAnalysisInteractionDelegate protocol methods.

```
interaction.delegate = self
```

If you don’t use a UIImageView object, inform the interaction object when the content area of the image changes while the interaction bounds don’t change. Implement the `ImageAnalysisInteractionDelegate` contentsRect(for:) protocol method to return the content area of the image. This keeps the Live Text highlights within the bounds of the image. Then use the setContentsRectNeedsUpdate() method to notify the interaction if the content area changes.

### Add a Live Text view to your image view in macOS

For macOS apps, add the Live Text interface by adding a view above the view containing the image. If you use an NSImageView to display the image, it handles the image content area calculations for you.

First create an instance of the ImageAnalysisOverlayView class.

```
let overlayView = ImageAnalysisOverlayView()
```

Then configure the overlay view to fit the bounds of the image. If your view is an image view, set the trackingImageView property so that the dimensions adjust when the scaling and alignment properties change.

```
overlayView.autoresizingMask = [.width, .height]
overlayView.frame = imageView.bounds
overlayView.trackingImageView = imageView
```

Add the overlay view above the image in the hierarchy. For example, add it as a subview of the view containing the image.

```
imageView.addSubview(overlayView)
```

To customize the interface, set the overlay view’s delegate to an object that implements the optional ImageAnalysisOverlayViewDelegate protocol methods.

```
overlayView.delegate = self
```

Implement the overlayView(_:shouldBeginAt:forAnalysisType:) protocol method to return `true` to begin the interaction.

```
func overlayView(_ overlayView: ImageAnalysisOverlayView, 
           shouldBeginAt point: CGPoint, forAnalysisType 
           analysisType: ImageAnalysisOverlayView.InteractionTypes) -> Bool { 
    overlayView.hasInteractiveItem(at: point) || 
    overlayView.hasActiveTextSelection 
}
```

If you aren’t using an NSImageView object, implement the `ImageAnalysisOverlayViewDelegate` contentsRect(for:) protocol method to return the content area of the image. Then use the setContentsRectNeedsUpdate() method to notify the overlay view if the content area of the image changes while the view bounds don’t change.

### Find items and start the interaction with an image

Process the image that your view displays using an ImageAnalyzer object. First, specify the types of items in the image you want to find when you create an ImageAnalyzer.Configuration object. For iOS apps, the analyzer recognizes both text and machine-readable QR codes in an image; for macOS apps, the analyzer recognizes text in an image.

```
let configuration = ImageAnalyzer.Configuration([.text, .machineReadableCode])
```

Then analyze the image by sending analyze(_:configuration:) to an ImageAnalyzer object, passing the image and the configuration. To improve performance, use a single shared instance of the analyzer throughout the app.

```
let analyzer = ImageAnalyzer()
let analysis = try? await analyzer.analyze(image, configuration: configuration)
```

For iOS apps, start the Live Text interface by setting the analysis property of the ImageAnalysisInteraction object to the results of the analyze method. For example, set the analysis property in the action method of a control that starts Live Text.

```
interaction.analysis = analysis
```

For macOS apps, start the Live Text interface by setting the analysis property of the ImageAnalysisOverlayView object.

```
overlayView.analysis = analysis
```

The standard Live Text menu appears when users click and hold items in the image. The user chooses actions from this menu, depending on the type of item.

### Customize behavior using interaction types

You can change the behavior of the interface by enabling types of interactions with items the analyzer finds in the image. If you set the interaction or overlay view preferredInteractionTypes property to automatic, users can interact with all types of items that the analyzer finds.

```
interaction.preferredInteractionTypes = .automatic
```

If you set the preferredInteractionTypes property to just textSelection, users can only select text in the image and then perform a basic text action, such as copying, translating, or sharing the text. For iOS apps, if the ImageAnalysisInteraction object’s allowLongPressForDataDetectorsInTextMode property is `true`, users can also touch and hold text that contains data (URLs, phone numbers, and email addresses) to perform a data-specific action.

For iOS apps, users can tap the Live Text button in the lower-right corner to switch to highlight mode. Then users can touch and hold data that the analyzer detects in text to perform a data-specific action, such as opening a URL, calling a phone number, or sending an email.

To let users interact with data that the analyzer detects in text in macOS, set the preferredInteractionTypes property to dataDetectors. Then users can hover over data in text to perform a data-specific action.

For iOS apps only, users can touch and hold QR codes and perform an action, depending on the payload, such as following an embedded link. To enable QR code interactions, set the ImageAnalyzer.Configuration structure’s analysisTypes property to machineReadableCode.

### Change the supplementary interface

You can modify the Live Text supplementary interface to conform better to the look of your app. The supplementary interface consists of the quick actions in the lower-left corner and the Live Text button in the lower-right corner of the interface.

To hide the supplementary interface, set the isSupplementaryInterfaceHidden to `false`. For iOS apps, if the allowLongPressForDataDetectorsInTextMode property is `true`, users can still touch and hold text to perform data-specific actions.

If your interface overlaps the supplementary interface, set the supplementaryInterfaceContentInsets property appropriately to move the quick actions and Live Text button.

If you want the supplementary interface to use a custom font, set the supplementaryInterfaceFont property. Quick actions use the specified font for text and font weight for symbols. For button size consistency, the Live Text interface ignores the point size.

### Specify recognized languages

By default the image analyzer attempts to recognize the user’s preferred languages. If you want the analyzer to consider other languages, set the locales property of the ImageAnalyzer.Configuration object.

To determine whether the image analyzer supports a language, check whether the array that the `ImageAnalyzer` supportedTextRecognitionLanguages class property returns includes the language ID.

For more information on language IDs, see Choosing localization regions and scripts.

## See Also

### Content recognition and interaction in images

class ImageAnalyzer

An object that finds items in images that people can interact with, such as subjects, text, and QR codes.

class ImageAnalysis

An object that represents the results of analyzing an image, and provides the input for the Live Text interface object.

class ImageAnalysisInteraction

An interface that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

