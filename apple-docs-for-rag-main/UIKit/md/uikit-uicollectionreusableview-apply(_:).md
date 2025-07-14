

- UIKit
- UICollectionReusableView
-  apply(\_:) 

Instance Method

# apply(\_:)

Applies the specified layout attributes to the view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func apply(_ layoutAttributes: UICollectionViewLayoutAttributes)
```

## Parameters 

`layoutAttributes`  

The layout attributes to apply.

## Discussion

The default implementation of this method does nothing.

If the layout object supports custom layout attributes, you can use this method to apply those attributes to the view. In such a case, the `layoutAttributes` parameter should contain an instance of a subclass of UICollectionViewLayoutAttributes. You do not need to override this method to support the standard layout attributes of the UICollectionViewLayoutAttributes class. The collection view applies those attributes automatically.

## See Also

### Managing layout changes

func preferredLayoutAttributesFitting(UICollectionViewLayoutAttributes) -> UICollectionViewLayoutAttributes

Gives the cell a chance to modify the attributes provided by the layout object.

func willTransition(from: UICollectionViewLayout, to: UICollectionViewLayout)

Tells your view that the layout object of the collection view is about to change.

func didTransition(from: UICollectionViewLayout, to: UICollectionViewLayout)

Tells your view that the layout object of the collection view changed.

