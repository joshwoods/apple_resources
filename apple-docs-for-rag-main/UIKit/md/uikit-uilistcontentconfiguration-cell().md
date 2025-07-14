

- UIKit
- UIListContentConfiguration
-  cell() 

Type Method

# cell()

Creates the default configuration you use to style a cell in a list.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func cell() -> UIListContentConfiguration
```

## Return Value

The default configuration for a cell in a list.

## Discussion

Create this configuration to update the content and styling of a cell in a list. When you apply this configuration to a cell, the cell displays one label, which resizes automatically based on the length of the text you provide and the device’s Dynamic Type and accessibility settings.

For an appearance consistent with system defaults, display your cell in a table view or collection view list that you configure with one of the following enumeration cases:

- UITableView.Style.plain

- UITableView.Style.grouped

- UITableView.Style.insetGrouped

- UICollectionLayoutListConfiguration.Appearance.plain

- UICollectionLayoutListConfiguration.Appearance.grouped

- UICollectionLayoutListConfiguration.Appearance.insetGrouped

Configure the background of your cell using one of the UIBackgroundConfiguration options below. Match the background of your cell to the corresponding table view or collection view styles as follows:

| Background configuration option | Matching table view or collection view styles |
|----|----|
| listPlainCell() | UITableView.Style.plain, UICollectionLayoutListConfiguration.Appearance.plain |
| listGroupedCell() | UITableView.Style.grouped, UITableView.Style.insetGrouped, UICollectionLayoutListConfiguration.Appearance.grouped, UICollectionLayoutListConfiguration.Appearance.insetGrouped |

## See Also

### Creating default cell configurations

static func subtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a list and contains subtitle text.

static func valueCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a list and contains side-by-side value text.

static func sidebarCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in a sidebar list.

static func sidebarSubtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a sidebar list and contains subtitle text.

static func accompaniedSidebarCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in an accompanied sidebar list.

static func accompaniedSidebarSubtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in an accompanied sidebar list and contains subtitle text.

