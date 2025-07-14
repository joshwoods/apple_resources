

- UIKit
- NSCollectionLayoutSection
-  contentInsetsReference 

Instance Property

# contentInsetsReference

The boundary to reference when defining content insets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var contentInsetsReference: UIContentInsetsReference { get set }
```

## Discussion

This property represents the reference point to use when defining contentInsets.

The default value of this property is UIContentInsetsReference.automatic, which means the section follows the layout configuration’s contentInsetsReference.

## See Also

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsets: NSDirectionalEdgeInsets

The amount of space between the content of the section and its boundaries.

var supplementaryContentInsetsReference: UIContentInsetsReference

The reference boundary for content insets on boundary supplementary items.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

