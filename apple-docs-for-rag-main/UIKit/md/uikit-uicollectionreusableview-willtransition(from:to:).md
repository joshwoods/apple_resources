

- UIKit
- UICollectionReusableView
-  willTransition(from:to:) 

Instance Method

# willTransition(from:to:)

Tells your view that the layout object of the collection view is about to change.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func willTransition(
    from oldLayout: UICollectionViewLayout,
    to newLayout: UICollectionViewLayout
)
```

## Parameters 

`oldLayout`  

The current layout object associated with the collection view.

`newLayout`  

The new layout object that is about to be applied to the collection view.

## Discussion

The default implementation of this method does nothing. Subclasses can override this method and use it to prepare for the change in layouts.

## See Also

### Managing layout changes

func preferredLayoutAttributesFitting(UICollectionViewLayoutAttributes) -> UICollectionViewLayoutAttributes

Gives the cell a chance to modify the attributes provided by the layout object.

func apply(UICollectionViewLayoutAttributes)

Applies the specified layout attributes to the view.

func didTransition(from: UICollectionViewLayout, to: UICollectionViewLayout)

Tells your view that the layout object of the collection view changed.

