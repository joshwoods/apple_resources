

- UIKit
- NSCollectionLayoutSection
-  contentInsets 

Instance Property

# contentInsets

The amount of space between the content of the section and its boundaries.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var contentInsets: NSDirectionalEdgeInsets { get set }
```

## See Also

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsetsReference: UIContentInsetsReference

The boundary to reference when defining content insets.

var supplementaryContentInsetsReference: UIContentInsetsReference

The reference boundary for content insets on boundary supplementary items.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

