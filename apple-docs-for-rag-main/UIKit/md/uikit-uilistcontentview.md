

- UIKit
-  UIListContentView 

Class

# UIListContentView

A content view for displaying list-based content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
class UIListContentView
```

## Overview

You use a list content view for displaying list-based content in a custom view hierarchy. You can embed a list content view manually in a custom cell or in a container view, like a UIStackView. You can use Auto Layout or manual layout techniques to size and position the view, and its height adjusts dynamically according to its width and the space it needs to display its content.

A list content view relies on its list content configuration to supply its styling and content. You create a list content view by passing in a UIListContentConfiguration to init(configuration:) (Swift) or initWithConfiguration: (Objective-C). To update the content view, you set a new configuration on it through its configuration property.

If you’re using a UICollectionView or UITableView, you don’t need to manually create a list content view to take advantage of the list configuration. Instead, you assign a UIListContentConfiguration to the contentConfiguration property of the cells, headers, or footers within those types.

## Topics

### Creating a list content view

convenience init(configuration: UIListContentConfiguration)

Creates a list content view with the specified content configuration.

init?(coder: NSCoder)

Creates a list content view from data in an unarchiver.

### Managing the content layout

var textLayoutGuide: UILayoutGuide?

A guide for positioning the primary text in the content view.

var secondaryTextLayoutGuide: UILayoutGuide?

A guide for positioning the secondary text in the content view.

var imageLayoutGuide: UILayoutGuide?

A guide for positioning the image in the content view.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
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
- UIContentView
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

### Content configurations

struct UIListContentConfiguration

A content configuration for a list-based content view.

protocol UIContentConfiguration

The requirements for an object that provides the configuration for a content view.

protocol UIContentView

The requirements for a content view that you create using a configuration.

