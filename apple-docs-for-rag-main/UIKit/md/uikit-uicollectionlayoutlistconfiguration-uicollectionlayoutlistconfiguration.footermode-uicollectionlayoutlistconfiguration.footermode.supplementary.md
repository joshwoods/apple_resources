

- UIKit
- UICollectionLayoutListConfiguration
- UICollectionLayoutListConfiguration.FooterMode
-  UICollectionLayoutListConfiguration.FooterMode.supplementary 

Case

# UICollectionLayoutListConfiguration.FooterMode.supplementary

A footer mode that uses supplementary views to show footers.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case supplementary
```

## Discussion

Choose this footer mode to use supplementary views with elementKindSectionFooter as the section footer.

By default, lists that use the UICollectionLayoutListConfiguration.Appearance.plain and UICollectionLayoutListConfiguration.Appearance.sidebarPlain list appearances use pinned footers. You must use this footer mode if you want to opt into this default pinning behavior.

## See Also

### Footer modes

case none

No footers are shown.

