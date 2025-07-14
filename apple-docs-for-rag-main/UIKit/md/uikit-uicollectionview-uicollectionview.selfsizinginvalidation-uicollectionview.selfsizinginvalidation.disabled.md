

- UIKit
- UICollectionView
- UICollectionView.SelfSizingInvalidation
-  UICollectionView.SelfSizingInvalidation.disabled 

Case

# UICollectionView.SelfSizingInvalidation.disabled

A mode that disables self-sizing invalidation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
case disabled
```

## Discussion

If you use this self-sizing invalidation mode, no sizing updates occur after calling invalidateIntrinsicContentSize() on a self-sizing cell or its contentView.

## See Also

### Constants

case enabled

A mode that enables manual self-sizing invalidation.

case enabledIncludingConstraints

A mode that enables automatic self-sizing invalidation after Auto Layout changes.

