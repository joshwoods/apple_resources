

- UIKit
- UIBackgroundConfiguration
-  listAccompaniedSidebarCell() 

Type Method

# listAccompaniedSidebarCell()

Creates the default configuration you use to style a cell in an accompanied sidebar list.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func listAccompaniedSidebarCell() -> UIBackgroundConfiguration
```

## Return Value

The default configuration for a cell in an accompanied sidebar list.

## Discussion

Create this configuration to update the styling for the background of a cell in a list. When you apply this configuration to a cell, the background of the cell matches the system default styling for a cell in an accompanied sidebar collection view list, including styling for highlighted and selected states. An accompanied sidebar collection view list is a list that’s in the primary column of a split view controller, accompanied by another list in the split view controller’s supplementary column.

For an appearance consistent with system defaults, use this background configuration for a cell in an accompanied sidebar collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.sidebar or UICollectionLayoutListConfiguration.Appearance.sidebarPlain enumeration case.

## See Also

### Creating cell background configurations

static func listPlainCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a plain list.

static func listGroupedCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a grouped list.

static func listSidebarCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a sidebar list.

