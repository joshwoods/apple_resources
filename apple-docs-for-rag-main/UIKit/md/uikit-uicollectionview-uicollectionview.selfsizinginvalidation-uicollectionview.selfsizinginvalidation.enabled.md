

- UIKit
- UICollectionView
- UICollectionView.SelfSizingInvalidation
-  UICollectionView.SelfSizingInvalidation.enabled 

Case

# UICollectionView.SelfSizingInvalidation.enabled

A mode that enables manual self-sizing invalidation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
case enabled
```

## Discussion

If you use this self-sizing invalidation mode, calling invalidateIntrinsicContentSize() on a self-sizing cell or its contentView causes the cell to resize if necessary.

## See Also

### Constants

case disabled

A mode that disables self-sizing invalidation.

case enabledIncludingConstraints

A mode that enables automatic self-sizing invalidation after Auto Layout changes.

