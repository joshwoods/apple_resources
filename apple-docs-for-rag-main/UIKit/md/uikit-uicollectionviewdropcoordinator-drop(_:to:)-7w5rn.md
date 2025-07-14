

- UIKit
- UICollectionViewDropCoordinator
-  drop(\_:to:) 

Instance Method

# drop(\_:to:)

Animates the item to an arbitrary location in your view hierarchy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    to target: UIDragPreviewTarget
) -> any UIDragAnimating
```

**Required**

## Parameters 

`dragItem`  

The item that you want to drop.

`target`  

The location at which to drop the item, specified as a point in a view. You can also use the UIDragPreviewTarget object to specify a final transform to apply to the content.

## Discussion

Use this method to animate drops to any view in your app. For example, you might use this method to drop items onto a tab bar or toolbar that’s part of your interface.

## See Also

### Animating Items to Their Destination

func drop(UIDragItem, toItemAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the collection view.

**Required**

func drop(UIDragItem, intoItemAt: IndexPath, rect: CGRect) -> any UIDragAnimating

Animates the item to the specified rectangle in the collection view.

**Required**

func drop(UIDragItem, to: UICollectionViewDropPlaceholder) -> any UICollectionViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

