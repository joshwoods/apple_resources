

- UIKit
- UITableViewDropCoordinator
-  drop(\_:toRowAt:) 

Instance Method

# drop(\_:toRowAt:)

Animates the item to the specified index path in the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    toRowAt indexPath: IndexPath
) -> any UIDragAnimating
```

**Required**

## Parameters 

`dragItem`  

The dragged item that you want to animate into position.

`indexPath`  

The index path to use as the destination for the animation.

## Mentioned in 

Supporting drag and drop in table views

## Discussion

Use this method to animate the dragged item to the specific location in the table view. Typically, you use this method for content that originated in the collection view and is moving to a new location.

## See Also

### Animating rows to their destination

func drop(UIDragItem, intoRowAt: IndexPath, rect: CGRect) -> any UIDragAnimating

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

func drop(UIDragItem, to: UITableViewDropPlaceholder) -> any UITableViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

