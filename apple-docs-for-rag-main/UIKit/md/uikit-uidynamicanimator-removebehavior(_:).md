

- UIKit
- UIDynamicAnimator
-  removeBehavior(\_:) 

Instance Method

# removeBehavior(\_:)

Removes a specified dynamic behavior from a dynamic animator.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func removeBehavior(_ behavior: UIDynamicBehavior)
```

## Parameters 

`behavior`  

The dynamic behavior instance that you want to remove from the animator.

The dynamic animator ignores your use of this method if you:

- Provide a `nil` value

- Provide a dynamic behavior instance that is not part of the animator’s behavior hierarchy

## See Also

### Initializing and managing a dynamic animator

init(referenceView: UIView)

Initializes a dynamic animator with a specified view as its reference view.

convenience init(collectionViewLayout: UICollectionViewLayout)

Initializes a dynamic animator with a specified collection view layout.

func items(in: CGRect) -> [any UIDynamicItem]

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

func addBehavior(UIDynamicBehavior)

Adds a dynamic behavior to a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

