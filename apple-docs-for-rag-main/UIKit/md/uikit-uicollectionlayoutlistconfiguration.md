

- UIKit
-  UICollectionLayoutListConfiguration 

Structure

# UICollectionLayoutListConfiguration

A configuration for creating a list layout.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UICollectionLayoutListConfiguration
```

## Overview

Use this configuration to create a list section for a compositional layout (UICollectionViewCompositionalLayout), or a layout containing only list sections. The following example shows how to create a compositional layout that contains only list sections by applying the same configuration to each section in the list layout:

```
let configuration = UICollectionLayoutListConfiguration(appearance: .sidebar)
let layout = UICollectionViewCompositionalLayout.list(using: configuration)
```

To implement different list configurations for different sections, use a compositional layout’s section provider to create each section with its own list configuration.

```
let layout = UICollectionViewCompositionalLayout() { sectionIndex, layoutEnvironment in

    var configuration = UICollectionLayoutListConfiguration(appearance: .insetGrouped)
    configuration.headerMode = sectionIndex == 0 ? .supplementary : .none

    let section = NSCollectionLayoutSection.list(using: configuration,
                                                 layoutEnvironment: layoutEnvironment)

    return section
}
```

## Topics

### Creating a list layout configuration

init(appearance: UICollectionLayoutListConfiguration.Appearance)

Creates a list layout configuration with the specified appearance.

### Configuring appearance

var appearance: UICollectionLayoutListConfiguration.Appearance

The overall appearance of the list.

var backgroundColor: UIColor?

The background color of the list.

enum Appearance

Constants that describe the appearance of the list.

### Configuring separators

var showsSeparators: Bool

A Boolean value that determines whether the list shows separators between cells.

var separatorConfiguration: UIListSeparatorConfiguration

The section’s preferred configuration for list separators.

struct UIListSeparatorConfiguration

A configuration that controls the list separator appearance in a list section.

var itemSeparatorHandler: UICollectionLayoutListConfiguration.ItemSeparatorHandler?

The closure that provides granular control over the list separator appearance of each item.

typealias ItemSeparatorHandler

A closure that provides granular control over list separator appearance.

### Configuring headers and footers

var headerMode: UICollectionLayoutListConfiguration.HeaderMode

The type of header to use for the list.

var footerMode: UICollectionLayoutListConfiguration.FooterMode

The type of footer to use for the list.

enum HeaderMode

Constants that describe the list’s header mode.

enum FooterMode

Constants that describe the list’s footer mode.

var headerTopPadding: CGFloat?

The amount of padding above each section header.

### Customizing swipe actions

var leadingSwipeActionsConfigurationProvider: UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider?

The closure that provides the set of actions to display when swiping on the leading edge of the cell.

var trailingSwipeActionsConfigurationProvider: UICollectionLayoutListConfiguration.SwipeActionsConfigurationProvider?

The closure that provides the set of actions to display when swiping on the trailing edge of the cell.

typealias SwipeActionsConfigurationProvider

A closure that configures the swipe actions for a cell.

### Managing content-hugging behavior

var contentHuggingElements: UICollectionLayoutListConfiguration.ContentHuggingElements

A setting that determines which type of items tightly hug their content.

struct ContentHuggingElements

Constants that determine which types of items in a collection view tightly hug their content.

## See Also

### Related Documentation

static func list(using: UICollectionLayoutListConfiguration, layoutEnvironment: any NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection

Creates a list section with the specified list configuration and layout environment.

### Creating a list layout

static func list(using: UICollectionLayoutListConfiguration) -> UICollectionViewCompositionalLayout

Creates a compositional layout that contains only list sections of the specified configuration.

