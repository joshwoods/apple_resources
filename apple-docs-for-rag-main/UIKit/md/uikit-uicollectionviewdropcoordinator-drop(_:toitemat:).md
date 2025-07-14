

- UIKit
- UICollectionViewDropCoordinator
-  drop(\_:toItemAt:) 

Instance Method

# drop(\_:toItemAt:)

Animates the item to the specified index path in the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    toItemAt indexPath: IndexPath
) -> any UIDragAnimating
```

**Required**

## Parameters 

`dragItem`  

The dragged item that you want to animate into position.

`indexPath`  

The index path to use as the destination for the animation.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

Use this method to animate the dragged item to the specific location in the collection view. Typically, you use this method for content that originated in the collection view and is moving to a new location.

## See Also

### Animating Items to Their Destination

func drop(UIDragItem, intoItemAt: IndexPath, rect: CGRect) -> any UIDragAnimating

Animates the item to the specified rectangle in the collection view.

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

func drop(UIDragItem, to: UICollectionViewDropPlaceholder) -> any UICollectionViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

