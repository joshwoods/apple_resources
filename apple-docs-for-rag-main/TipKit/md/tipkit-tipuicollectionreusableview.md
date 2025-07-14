

- TipKit
-  TipUICollectionReusableView 

Class

# TipUICollectionReusableView

A UICollectionReusableView subclass that represents a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class TipUICollectionReusableView
```

## Overview

You create a tip view by providing a tip and an optional arrow edge. The tip is a type that conforms to the Tip protocol. The arrow edge is a directional arrow pointing away from the tip.

## Topics

### Initializers

init?(coder: NSCoder)

init(frame: CGRect)

### Instance Properties

var cornerRadius: CGFloat

Corner radius for the tip view.

var imageSize: CGSize

Size of the image displayed in the tip view.

var imageStyle: (any ShapeStyle)?

Foreground style for the tip’s image.

var viewStyle: any TipViewStyle

The given style for TipView within the view hierarchy

### Instance Methods

func configureTip(any Tip, arrowEdge: Edge?, actionHandler: (Tips.Action) -> Void) -> Self

Configures a reusable view with a tip view embedded.

## Relationships

### Inherits From

- UICollectionReusableView

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

### UIKit Views

class TipUIView

A user interface element that represents a tip in UIKit applications.

class TipUIPopoverViewController

A view controller that displays a popover tip in UIKit applications.

class TipUICollectionViewCell

A collection view cell that embeds a tip.

