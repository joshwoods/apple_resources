

- UIKit
- NSCollectionLayoutSection
-  supplementaryContentInsetsReference 

Instance Property

# supplementaryContentInsetsReference

The reference boundary for content insets on boundary supplementary items.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var supplementaryContentInsetsReference: UIContentInsetsReference { get set }
```

## Discussion

This property represents the reference boundary to use when defining contentInsets on NSCollectionLayoutBoundarySupplementaryItem objects.

The default value of this property is UIContentInsetsReference.automatic, which means any insets specified on a NSCollectionLayoutBoundarySupplementaryItem follow the layout configuration’s contentInsetsReference.

## See Also

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsets: NSDirectionalEdgeInsets

The amount of space between the content of the section and its boundaries.

var contentInsetsReference: UIContentInsetsReference

The boundary to reference when defining content insets.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

