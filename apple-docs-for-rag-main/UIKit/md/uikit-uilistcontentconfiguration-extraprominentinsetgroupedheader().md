

- UIKit
- UIListContentConfiguration
-  extraProminentInsetGroupedHeader() 

Type Method

# extraProminentInsetGroupedHeader()

Creates the default configuration you use to style an extra prominent header in an inset grouped list.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func extraProminentInsetGroupedHeader() -> UIListContentConfiguration
```

## Return Value

The default configuration for an extra prominent header in an inset grouped list.

## Discussion

Create this configuration to update the content and styling of a header in a table view or collection view list.

For an appearance consistent with system defaults, display your header in a table view or collection view list that you configure with one of the following enumeration cases:

- UITableView.Style.insetGrouped

- UICollectionLayoutListConfiguration.Appearance.insetGrouped

Configure the background of your header using one of the UIBackgroundConfiguration options below. Match the background of your header to the corresponding table view or collection view styles as follows:

| Background configuration option | Matching table view or collection view styles |
|----|----|
| listGroupedHeaderFooter() | UITableView.Style.insetGrouped, UICollectionLayoutListConfiguration.Appearance.insetGrouped |

## See Also

### Creating header and footer configurations

static func plainHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a plain list.

static func plainFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a plain list.

static func groupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a grouped list.

static func groupedFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a grouped list.

static func prominentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a prominent header in an inset grouped list.

static func sidebarHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a sidebar list.

