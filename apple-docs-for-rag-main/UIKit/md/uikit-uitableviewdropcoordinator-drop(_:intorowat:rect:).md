

- UIKit
- UITableViewDropCoordinator
-  drop(\_:intoRowAt:rect:) 

Instance Method

# drop(\_:intoRowAt:rect:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    intoRowAt indexPath: IndexPath,
    rect: CGRect
) -> any UIDragAnimating
```

**Required**

## Parameters 

`dragItem`  

The dragged item that you want to animate into position.

`indexPath`  

The index path in the table view at which to incorporate the item.

`rect`  

The destination rectangle to use for the animation. Specify the rectangle in the coordinate system of the cell at the specified `indexPath`. UIKit animates the drag item to the specified rectangle.

## Discussion

Use this method to animate drops where you incorporate the dragged items into another item of your table view. For example, when incorporating items into a folder, you would use this method to animate the items in a way that makes it look like they were placed into the folder.

## See Also

### Animating rows to their destination

func drop(UIDragItem, toRowAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the table view.

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

func drop(UIDragItem, to: UITableViewDropPlaceholder) -> any UITableViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

