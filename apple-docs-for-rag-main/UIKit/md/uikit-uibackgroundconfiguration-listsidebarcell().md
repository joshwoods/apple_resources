

- UIKit
- UIBackgroundConfiguration
-  listSidebarCell() 

Type Method

# listSidebarCell()

Creates the default configuration you use to style a cell in a sidebar list.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalysttvOS 14.0+visionOS

``` source
static func listSidebarCell() -> UIBackgroundConfiguration
```

## Return Value

The default configuration for a cell in a sidebar list.

## Discussion

Create this configuration to update the styling for the background of a cell in a list. When you apply this configuration to a cell, the background of the cell matches the system default styling for a cell in a sidebar collection view list, including styling for highlighted and selected states.

For an appearance consistent with system defaults, use this background configuration for a cell in a collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.sidebar or UICollectionLayoutListConfiguration.Appearance.sidebarPlain enumeration case.

## See Also

### Creating cell background configurations

static func listPlainCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a plain list.

static func listGroupedCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in a grouped list.

static func listAccompaniedSidebarCell() -> UIBackgroundConfiguration

Creates the default configuration you use to style a cell in an accompanied sidebar list.

