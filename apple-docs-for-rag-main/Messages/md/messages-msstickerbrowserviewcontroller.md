

- Messages
-  MSStickerBrowserViewController 

Class

# MSStickerBrowserViewController

A view controller that provides dynamic content to the standard sticker browser.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class MSStickerBrowserViewController
```

## Overview

Use the MSStickerBrowserViewController to present the standard sticker browser. This browser provides drag-and-drop functionality. The user can press and hold a sticker to peel it from the browser, then drag the sticker to any balloon in the transcript. The user can also tap stickers to add them to the Messages app’s input field.

By default, the sticker browser view controller acts as the data source for its MSStickerBrowserView view (see the stickerBrowserView property). This lets you dynamically change the list of stickers at runtime. You can also customize the size of the stickers inside the browser.

### Setting the Sticker Browser as Your Root View

To use the sticker browser view controller as your extension’s root view, perform the following steps:

1.  Create a custom subclass of the MSStickerBrowserViewController class. For more information, see the subclassing notes.

2.  In Interface Builder, add a container view to your extension’s initial scene and pin it to fill the root view as desired. For more information on setting up a container view, see Configuring a Container in Interface Builder.

3.  In the Identity inspector, set the embedded view controller’s class to your custom MSStickerBrowserViewController subclass.

By using an MSMessagesAppViewController instance as the extension’s root view controller, this approach ensures that the root view controller can respond to important messages from the system, while the contained sticker browser view controller focuses on managing your stickers.

### Subclassing Notes

By default, this controller sets itself as its sticker browser view’s data source. You must either provide another data source, or implement both numberOfStickers(in:) and stickerBrowserView(_:stickerAt:).

For more information, see MSStickerBrowserViewDataSource.

## Topics

### Working with Stickers

init(stickerSize: MSStickerSize)

Creates a new sticker browser view controller with stickers of the provided size.

var stickerBrowserView: MSStickerBrowserView

The sticker browser view managed by this controller.

var stickerSize: MSStickerSize

A constant that indicates the size of the stickers.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MSStickerBrowserViewDataSource
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Custom sticker packs

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

Enable your Sticker pack or iMessage app in the media context.

Adding your sticker packs to Messages

Drag and drop your sticker pack into the Stickers asset catalog to let people access your stickers from Messages.

class MSStickerBrowserView

A browser view that displays a dynamically generated list of stickers.

class MSStickerView

A view for displaying a sticker.

enum MSStickerSize

The size of the stickers in the browser view.

