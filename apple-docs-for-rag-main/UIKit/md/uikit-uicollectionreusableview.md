

- UIKit
-  UICollectionReusableView 

Class

# UICollectionReusableView

A view that defines the behavior for all cells and supplementary views presented by a collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollectionReusableView
```

## Overview

Reusable views are so named because the collection view places them on a reuse queue rather than deleting them when they’re scrolled out of the visible bounds. Such a view can then be retrieved and repurposed for a different set of content.

### Subclassing notes

This class is intended to be subclassed. Most methods defined by this class have minimal or no implementations. You aren’t required to override any of the methods but can do so in cases where you want to respond to changes in the view’s usage or layout.

## Topics

### Reusing cells

var reuseIdentifier: String?

A string that identifies the purpose of the view.

func prepareForReuse()

Performs any clean up necessary to prepare the view for use again.

### Managing layout changes

func preferredLayoutAttributesFitting(UICollectionViewLayoutAttributes) -> UICollectionViewLayoutAttributes

Gives the cell a chance to modify the attributes provided by the layout object.

func apply(UICollectionViewLayoutAttributes)

Applies the specified layout attributes to the view.

func willTransition(from: UICollectionViewLayout, to: UICollectionViewLayout)

Tells your view that the layout object of the collection view is about to change.

func didTransition(from: UICollectionViewLayout, to: UICollectionViewLayout)

Tells your view that the layout object of the collection view changed.

## Relationships

### Inherits From

- UIView

### Inherited By

- UICollectionViewCell

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

### Cells

class UICollectionViewCell

A single data item when that item is within the collection view’s visible bounds.

class UICollectionViewListCell

A collection view cell that provides list features and default styling.

