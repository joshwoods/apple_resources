

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:sceneActivationConfigurationForItemAt:point:) 

Instance Method

# collectionView(\_:sceneActivationConfigurationForItemAt:point:)

Returns a scene activation configuration that allows the cell to expand into a new scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    sceneActivationConfigurationForItemAt indexPath: IndexPath,
    point: CGPoint
) -> UIWindowScene.ActivationConfiguration?
```

## Parameters 

`collectionView`  

The collection view.

`indexPath`  

The index path of the cell with which the user is interacting.

`point`  

The location of the interaction in the collection view’s coordinate space.

## Return Value

A UIWindowScene.ActivationConfiguration object that facilitates expanding the cell into a new scene. Return `nil` to prevent the interaction from starting.

