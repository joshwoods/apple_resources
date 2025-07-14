

- UIKit
- UIBackgroundConfiguration
-  listSidebarHeader() 

Type Method

# listSidebarHeader()

Creates the default configuration you use to style a sidebar list header.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac CatalystvisionOS

``` source
static func listSidebarHeader() -> UIBackgroundConfiguration
```

## Return Value

The default configuration for a sidebar list header.

## Discussion

Create this configuration to update the styling for the background of a header or footer in a table view or collection view list. When you apply this configuration, the background of the header or footer matches the system default styling for a header or footer in a sidebar list.

For an appearance consistent with system defaults, use this background configuration for a header or footer in a collection view list that you configure with the UICollectionLayoutListConfiguration.Appearance.sidebar enumeration case.

## See Also

### Creating header and footer background configurations

static func listPlainHeaderFooter() -> UIBackgroundConfiguration

Creates the default configuration you use to style a plain list header or footer.

Deprecated

static func listGroupedHeaderFooter() -> UIBackgroundConfiguration

Creates the default configuration you use to style a grouped list header or footer.

Deprecated

