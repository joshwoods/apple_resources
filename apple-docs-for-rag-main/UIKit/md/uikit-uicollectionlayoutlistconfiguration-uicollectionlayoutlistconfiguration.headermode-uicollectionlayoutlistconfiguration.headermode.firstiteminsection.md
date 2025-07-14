

- UIKit
- UICollectionLayoutListConfiguration
- UICollectionLayoutListConfiguration.HeaderMode
-  UICollectionLayoutListConfiguration.HeaderMode.firstItemInSection 

Case

# UICollectionLayoutListConfiguration.HeaderMode.firstItemInSection

A header mode that styles the first item in a section as a header.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case firstItemInSection
```

## Discussion

Choose this header mode when you’re using hierarchical data sources if you want to be able to expand and collapse the header.

When you use this header mode, a UICollectionViewListCell object that appears as the first item in the section automatically uses a header appearance. When you configure your data source, make sure to account for the fact that the first item in the section (at index `0`) represents the header, and the actual items in the section start at index `1`.

By default, lists that use the UICollectionLayoutListConfiguration.Appearance.plain and UICollectionLayoutListConfiguration.Appearance.sidebarPlain list appearances use pinned headers. If you want to opt into this default pinning behavior, use the UICollectionLayoutListConfiguration.HeaderMode.supplementary header mode instead.

## See Also

### Header modes

case none

No headers are shown.

case supplementary

A header mode that uses supplementary views to show headers.

