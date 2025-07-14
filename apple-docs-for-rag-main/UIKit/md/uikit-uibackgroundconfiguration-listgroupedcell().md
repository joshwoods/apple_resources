

- UIKit
- UIBackgroundConfiguration
-  listGroupedCell() 

Type Method

# listGroupedCell()

Creates the default configuration you use to style a cell in a grouped list.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalysttvOS 14.0–18.0DeprecatedvisionOS

``` source
static func listGroupedCell() -> UIBackgroundConfiguration
```

## Return Value

The default configuration for a cell in a grouped list.

## Discussion

Create this configuration to update the styling for the background of a cell in a list. When you apply this configuration to a cell, the background of the cell matches the system default styling for a grouped cell, including styling for highlighted and selected states.

For an appearance consistent with system defaults, use this background configuration for a cell in these contexts:

- A table view that you configure with the UITableView.Style.grouped or UITableView.Style.insetGrouped enumeration case.

- A collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.grouped or UICollectionLayoutListConfiguration.Appearance.insetGrouped enumeration case.

## See Also

### Creating cell background configurations

static func listPlainCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a plain list.

static func listSidebarCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a sidebar list.

static func listAccompaniedSidebarCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in an accompanied sidebar list.

