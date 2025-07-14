

- Messages
-  MSStickerBrowserView 

Class

# MSStickerBrowserView

A browser view that displays a dynamically generated list of stickers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class MSStickerBrowserView
```

## Overview

Use the MSStickerBrowserView to display a dynamically generated list of stickers. The browser provides drag-and-drop functionality. The user can press and hold a sticker to peel it from the browser, then drag the sticker to any balloon in the transcript. The user can also tap stickers to add them to the Messages app’s input field.

The sticker browser presents the stickers provided by its dataSource property. The data source can dynamically change the list of stickers at runtime. You can also customize the size of the stickers inside the browser.

If you create an MSStickerBrowserViewController object, it automatically creates and displays a sticker browser view with stickers of the specified size. The controller is automatically set as the browser’s data source. Alternatively, you can instantiate your own sticker browser view, letting you customize the size of both the browser and the stickers; however, you need to provide your own data source.

If you need additional customizations, you must build your own user interface using MSStickerView objects.

If you are simply presenting a static list of stickers using the default browser interface, consider building a Sticker Pack Application instead. For more information, see Messages.

## Topics

### Creating Sticker Browser Views

init(frame: CGRect)

Creates a new sticker browser containing medium-sized stickers.

init(frame: CGRect, stickerSize: MSStickerSize)

Creates a new sticker browser containing stickers of the specified size.

### Managing the Sticker Collection Contents

var dataSource: (any MSStickerBrowserViewDataSource)?

The sticker browser’s data source.

protocol MSStickerBrowserViewDataSource

The protocol for dynamically providing stickers to a browser view.

func reloadData()

Asks the sticker browser to reload its data from the data source.

### Managing the Browser’s Appearance

var contentInset: UIEdgeInsets

The distance that the content is inset from the edge of the browser view.

var contentOffset: CGPoint

The distance that the content is offset from the browser’s origin.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset distance between the content and the browser’s origin.

var stickerSize: MSStickerSize

The size of the stickers in the browser.

### Constants

enum MSStickerSize

The size of the stickers in the browser view.

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

class MSStickerView

A view for displaying a sticker.

enum MSStickerSize

The size of the stickers in the browser view.

