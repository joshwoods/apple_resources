

- UIKit
- UIDynamicAnimator
-  init(referenceView:) 

Initializer

# init(referenceView:)

Initializes a dynamic animator with a specified view as its reference view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
init(referenceView view: UIView)
```

## Parameters 

`view`  

The view for the dynamic animator, called the *reference view*.

## Return Value

The initialized dynamic animator, or `nil` if there was a problem initializing the object.

## Discussion

When you initialize a dynamic animator with this method, the behaviors (and their dynamic items) that you add to the animator employ the reference view’s coordinate system.

## See Also

### Initializing and managing a dynamic animator

convenience init(collectionViewLayout: UICollectionViewLayout)

Initializes a dynamic animator with a specified collection view layout.

func items(in: CGRect) -> [any UIDynamicItem]

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

func addBehavior(UIDynamicBehavior)

Adds a dynamic behavior to a dynamic animator.

func removeBehavior(UIDynamicBehavior)

Removes a specified dynamic behavior from a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

