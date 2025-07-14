

- UIKit
- UIDynamicAnimator
-  init(collectionViewLayout:) 

Initializer

# init(collectionViewLayout:)

Initializes a dynamic animator with a specified collection view layout.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
convenience init(collectionViewLayout layout: UICollectionViewLayout)
```

## Parameters 

`layout`  

The collection view layout for the dynamic animator, serving as the reference view for a dynamic animator in collection-view mode.

## Return Value

The initialized dynamic animator, or `nil` if there was a problem initializing the object.

## Discussion

When you initialize a dynamic animator with this method, the behaviors (and their dynamic items) that you add to the animator employ the collection view layout’s coordinate system.

## See Also

### Initializing and managing a dynamic animator

init(referenceView: UIView)

Initializes a dynamic animator with a specified view as its reference view.

func items(in: CGRect) -> [any UIDynamicItem]

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

func addBehavior(UIDynamicBehavior)

Adds a dynamic behavior to a dynamic animator.

func removeBehavior(UIDynamicBehavior)

Removes a specified dynamic behavior from a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

