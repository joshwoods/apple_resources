

- UIKit
-  UICollectionViewCell 

Class

# UICollectionViewCell

A single data item when that item is within the collection view’s visible bounds.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollectionViewCell
```

## Overview

You can use UICollectionViewCell as-is or subclass it to add additional properties and methods. The layout and presentation of cells is managed by the collection view and its corresponding layout object.

To configure the content and appearance of your cell, you can set its contentConfiguration and backgroundConfiguration. Alternatively, add the views needed to present the data item’s content as subviews to the view in the contentView property. Don’t directly add subviews to the cell itself. The cell manages multiple layers of content, of which the content view is only one. In addition to the content view, the cell manages two background views that display the cell in its selected and unselected states.

You typically don’t create instances of this class yourself. Instead, you register your specific cell subclass (or a nib file containing a configured instance of your class) using a cell registration. When you want a new instance of your cell class, call the dequeueConfiguredReusableCell(using:for:item:) (Swift) or dequeueConfiguredReusableCellWithRegistration:forIndexPath:item: (Objective-C) method of the collection view object to retrieve one.

## Topics

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The view that displays behind the cell’s other content.

var selectedBackgroundView: UIView?

The view that displays just above the background view for a selected cell.

### Managing the content

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the cell.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its content configuration when its state changes.

var contentView: UIView

The main view that you add your cell’s custom content to.

### Managing the state

var configurationState: UICellConfigurationState

The current configuration state of the cell.

func setNeedsUpdateConfiguration()

Informs the cell to update its configuration for its current state.

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the cell’s configuration using the current state.

var isSelected: Bool

The selection state of the cell.

var isHighlighted: Bool

The highlight state of the cell.

### Managing drag state changes

func dragStateDidChange(UICollectionViewCell.DragState)

Called when the drag state of the cell changes.

enum DragState

Constants indicating the current state of the drag operation.

## Relationships

### Inherits From

- UICollectionReusableView

### Inherited By

- UICollectionViewListCell

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

class UICollectionViewListCell

A collection view cell that provides list features and default styling.

class UICollectionReusableView

A view that defines the behavior for all cells and supplementary views presented by a collection view.

