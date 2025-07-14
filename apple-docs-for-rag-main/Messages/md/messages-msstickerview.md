

- Messages
-  MSStickerView 

Class

# MSStickerView

A view for displaying a sticker.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class MSStickerView
```

## Overview

Use the MSStickerView class to display stickers. The sticker view also provides drag-and-drop functionality. The user can press and hold a sticker to peel it from the view, and then drag the sticker to any balloon in the transcript.

## Topics

### Working with Sticker Views

init(frame: CGRect, sticker: MSSticker?)

Initializes a new sticker view with the provided sticker and frame.

var sticker: MSSticker?

The displayed sticker object.

### Controlling Sticker Animation

var animationDuration: TimeInterval

The amount of time it takes to complete the sticker’s animation.

func isAnimating() -> Bool

Returns a Boolean value that indicates whether the sticker is animating.

func startAnimating()

Starts the sticker’s animation, beginning with the first frame.

func stopAnimating()

Stops the sticker’s animation.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Custom sticker packs

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

Enable your Sticker pack or iMessage app in the media context.

Adding your sticker packs to Messages

Drag and drop your sticker pack into the Stickers asset catalog to let people access your stickers from Messages.

class MSStickerBrowserViewController

A view controller that provides dynamic content to the standard sticker browser.

class MSStickerBrowserView

A browser view that displays a dynamically generated list of stickers.

enum MSStickerSize

The size of the stickers in the browser view.

