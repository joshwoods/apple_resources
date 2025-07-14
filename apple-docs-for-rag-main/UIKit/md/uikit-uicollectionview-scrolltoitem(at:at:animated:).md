

- UIKit
- UICollectionView
-  scrollToItem(at:at:animated:) 

Instance Method

# scrollToItem(at:at:animated:)

Scrolls the collection view contents until the specified item is visible.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scrollToItem(
    at indexPath: IndexPath,
    at scrollPosition: UICollectionView.ScrollPosition,
    animated: Bool
)
```

## Parameters 

`indexPath`  

The index path of the item to scroll into view.

`scrollPosition`  

An option that specifies where the item should be positioned when scrolling finishes. For a list of possible values, see UICollectionView.ScrollPosition.

`animated`  

Specify true to animate the scrolling behavior or false to adjust the scroll view’s visible content immediately.

## See Also

### Scrolling an item into view

struct ScrollPosition

Constants that indicate how to scroll an item into the visible portion of the collection view.

enum ScrollDirection

Constants that indicate the direction of scrolling for the layout.

