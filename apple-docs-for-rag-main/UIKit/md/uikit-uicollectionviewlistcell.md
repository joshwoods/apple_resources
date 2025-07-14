

- UIKit
-  UICollectionViewListCell 

Class

# UICollectionViewListCell

A collection view cell that provides list features and default styling.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
class UICollectionViewListCell
```

## Overview

A list cell represents an individual item that might appear in a list. List cells provide built-in support for indentation, and the ability to add cell accessories (UICellAccessory) for visual adornment or to support user interactions with the cell.

You can use a list cell in any type of layout. Using a list cell inside a list enables additional list-specific behavior for the cells. For example, in a list section or layout, you can define separator alignment between list cells, and configure swipe actions for each cell’s leading and trailing edges. You create an individual list section using list(using:layoutEnvironment:), or a full list layout using list(using:).

You can use a list cell’s defaultContentConfiguration() (Swift) or defaultContentConfiguration (Objective-C) to get a list content configuration that has preconfigured default styling. After you get the default configuration, you assign your content to it, customize any other properties, and assign it to the cell as the current content configuration. For customization options, see UIListContentConfiguration.

- Swift
- Objective-C

```
var content = cell.defaultContentConfiguration()

// Configure content.
content.image = UIImage(systemName: "star")
content.text = "Favorites"

// Customize appearance.
content.imageProperties.tintColor = .purple

cell.contentConfiguration = content
```

```
UIListContentConfiguration *content = [cell defaultContentConfiguration];

// Configure content.
[content setImage:[UIImage systemImageNamed:@"star"]];
[content setText:@"Favorites"];

// Customize appearance.
[content.imageProperties setTintColor:[UIColor purpleColor]];

[cell setContentConfiguration:content];
```

Alternatively, you can set your content through your own custom subviews using the cell’s contentView.

## Topics

### Getting a configuration

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the cell’s style.

### Managing cell accessories

var accessories: [UICellAccessory]

An array of the accessories that decorate the cell.

struct UICellAccessory

An accessory in a collection view list cell.

### Customizing layout

var indentationLevel: Int

The level of indentation for the cell.

var indentationWidth: CGFloat

The width of an indentation level.

var indentsAccessories: Bool

A Boolean value that detemines whether the cell indents accessories on the leading side.

var separatorLayoutGuide: UILayoutGuide

A guide for laying out separators in relation to the primary content in the cell.

## Relationships

### Inherits From

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

class UICollectionReusableView

A view that defines the behavior for all cells and supplementary views presented by a collection view.

