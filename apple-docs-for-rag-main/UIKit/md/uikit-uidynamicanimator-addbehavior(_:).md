

- UIKit
- UIDynamicAnimator
-  addBehavior(\_:) 

Instance Method

# addBehavior(\_:)

Adds a dynamic behavior to a dynamic animator.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func addBehavior(_ behavior: UIDynamicBehavior)
```

## Parameters 

`behavior`  

The dynamic behavior instance you are adding.

The dynamic animator ignores your use of this method if you:

- Provide a `nil` value

- Provide a behavior instance that you’ve already added to the animator at the same level in the behavior hierarchy

Important

The dynamic animator raises an exception if you provide a behavior instance that you’ve already added to the animator at a different level in the behavior hierarchy.

## See Also

### Initializing and managing a dynamic animator

init(referenceView: UIView)

Initializes a dynamic animator with a specified view as its reference view.

convenience init(collectionViewLayout: UICollectionViewLayout)

Initializes a dynamic animator with a specified collection view layout.

func items(in: CGRect) -> [any UIDynamicItem]

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

func removeBehavior(UIDynamicBehavior)

Removes a specified dynamic behavior from a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

