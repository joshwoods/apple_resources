

- UIKit
- UICollectionViewCompositionalLayoutConfiguration
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

The default value of this property is UIContentInsetsReference.safeArea.

## See Also

### Configuring spacing

var interSectionSpacing: CGFloat

The amount of space between the sections in the layout.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

