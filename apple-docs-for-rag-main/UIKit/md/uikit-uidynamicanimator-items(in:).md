

- UIKit
- UIDynamicAnimator
-  items(in:) 

Instance Method

# items(in:)

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func items(in rect: CGRect) -> [any UIDynamicItem]
```

## Parameters 

`rect`  

The rectangle you are interested in.

## Return Value

The dynamic items, from the animator’s behaviors, that intersect the specified rectangle.

## Discussion

The coordinate system that pertains to the `rect` parameter depends on how you initialized the animator, as described in the Overview in this document.

## See Also

### Initializing and managing a dynamic animator

init(referenceView: UIView)

Initializes a dynamic animator with a specified view as its reference view.

convenience init(collectionViewLayout: UICollectionViewLayout)

Initializes a dynamic animator with a specified collection view layout.

func addBehavior(UIDynamicBehavior)

Adds a dynamic behavior to a dynamic animator.

func removeBehavior(UIDynamicBehavior)

Removes a specified dynamic behavior from a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

