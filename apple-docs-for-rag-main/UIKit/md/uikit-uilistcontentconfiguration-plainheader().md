

- UIKit
- UIListContentConfiguration
-  plainHeader() 

Type Method

# plainHeader()

Creates the default configuration you use to style a header in a plain list.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalysttvOS 14.0–18.0DeprecatedvisionOS

``` source
static func plainHeader() -> UIListContentConfiguration
```

## Return Value

The default configuration for a header in a plain list.

## Discussion

Create this configuration to update the content and styling of a header in a table view or collection view list.

For an appearance consistent with system defaults, display your header in a table view or collection view list that you configure with one of the following enumeration cases:

- UITableView.Style.plain

- UICollectionLayoutListConfiguration.Appearance.plain

- UICollectionLayoutListConfiguration.Appearance.sidebarPlain

Configure the background of your header using one of the UIBackgroundConfiguration options below. Match the background of your header to the corresponding table view or collection view styles as follows:

| Background configuration option | Matching table view or collection view styles |
|----|----|
| listPlainHeaderFooter() | UITableView.Style.plain, UICollectionLayoutListConfiguration.Appearance.plain, UICollectionLayoutListConfiguration.Appearance.sidebarPlain |

## See Also

### Creating header and footer configurations

static func plainFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a plain list.

static func groupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a grouped list.

static func groupedFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a grouped list.

static func prominentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a prominent header in an inset grouped list.

static func extraProminentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style an extra prominent header in an inset grouped list.

static func sidebarHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a sidebar list.

