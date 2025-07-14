

- UIKit
- UICollectionLayoutListConfiguration
- UICollectionLayoutListConfiguration.HeaderMode
-  UICollectionLayoutListConfiguration.HeaderMode.supplementary 

Case

# UICollectionLayoutListConfiguration.HeaderMode.supplementary

A header mode that uses supplementary views to show headers.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case supplementary
```

## Discussion

Choose this header mode to use supplementary views with elementKindSectionHeader as the section header.

By default, lists that use the UICollectionLayoutListConfiguration.Appearance.plain and UICollectionLayoutListConfiguration.Appearance.sidebarPlain list appearances use pinned headers. You must use this header mode if you want to opt into this default pinning behavior.

## See Also

### Header modes

case none

No headers are shown.

case firstItemInSection

A header mode that styles the first item in a section as a header.

