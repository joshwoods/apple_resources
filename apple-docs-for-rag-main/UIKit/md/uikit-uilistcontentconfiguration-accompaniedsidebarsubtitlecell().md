

- UIKit
- UIListContentConfiguration
-  accompaniedSidebarSubtitleCell() 

Type Method

# accompaniedSidebarSubtitleCell()

Creates the default configuration you use to style a cell that’s in an accompanied sidebar list and contains subtitle text.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func accompaniedSidebarSubtitleCell() -> UIListContentConfiguration
```

## Return Value

The default configuration for a cell that’s in an accompanied sidebar list and contains subtitle text.

## Discussion

Create this configuration to update the content and styling of a cell in an accompanied sidebar collection view list, where the list is in the primary column of a split view controller, accompanied by another list in the split view controller’s supplementary column. When you apply this configuration to a cell, the cell displays one primary label and one subtitle label below the primary label. Both labels resize automatically based on the length of the text you provide and the device’s Dynamic Type and accessibility settings.

For an appearance consistent with system defaults, display your cell in an accompanied sidebar collection view list that you configure with one of the following enumeration cases:

- UICollectionLayoutListConfiguration.Appearance.sidebar

- UICollectionLayoutListConfiguration.Appearance.sidebarPlain

Configure the background of your cell using one of the UIBackgroundConfiguration options below. Match the background of your cell to the corresponding table view or collection view styles as follows:

| Background configuration option | Matching table view or collection view styles |
|----|----|
| listAccompaniedSidebarCell() | UICollectionLayoutListConfiguration.Appearance.sidebar, UICollectionLayoutListConfiguration.Appearance.sidebarPlain |

## See Also

### Creating default cell configurations

static func cell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in a list.

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

