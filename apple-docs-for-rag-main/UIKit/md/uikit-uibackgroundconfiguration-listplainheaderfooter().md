

- UIKit
- UIBackgroundConfiguration
-  listPlainHeaderFooter() 

Type Method

# listPlainHeaderFooter()

Creates the default configuration you use to style a plain list header or footer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalysttvOS 14.0–18.0DeprecatedvisionOS

``` source
static func listPlainHeaderFooter() -> UIBackgroundConfiguration
```

## Return Value

The default configuration for a plain list header or footer.

## Discussion

Create this configuration to update the styling for the background of a header or footer in a table view or collection view list. When you apply this configuration, the background of the header or footer matches the system default styling for a header or footer in a plain list.

For an appearance consistent with system defaults, use this background configuration for a header or footer in these contexts:

- A table view that you configure with the UITableView.Style.plain enumeration case.

- A collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.plain or UICollectionLayoutListConfiguration.Appearance.sidebarPlain enumeration cases.

## See Also

### Creating header and footer background configurations

static func listGroupedHeaderFooter() -> UIBackgroundConfiguration

Creates the default configuration you use to style a grouped list header or footer.

Deprecated

static func listSidebarHeader() -> UIBackgroundConfiguration

Creates the default configuration you use to style a sidebar list header.

Deprecated

