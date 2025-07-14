

- UIKit
- UIListContentConfiguration
-  sidebarHeader() 

Type Method

# sidebarHeader()

Creates the default configuration you use to style a header in a sidebar list.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalystvisionOS

``` source
static func sidebarHeader() -> UIListContentConfiguration
```

## Return Value

The default configuration for a header in a sidebar list.

## Discussion

Create this configuration to update the content and styling of a header in a sidebar collection view list.

For an appearance consistent with system defaults, display your header in a sidebar collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.sidebar enumeration case.

Configure the background of your cell using one of the UIBackgroundConfiguration options below. Match the background of your cell to the corresponding table view or collection view styles as follows:

| Background configuration option | Matching table view or collection view styles |
|----|----|
| listSidebarHeader() | UICollectionLayoutListConfiguration.Appearance.sidebar |

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

static func extraProminentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style an extra prominent header in an inset grouped list.

