

- UIKit
- UICollectionView
-  numberOfItems(inSection:) 

Instance Method

# numberOfItems(inSection:)

Fetches the count of items in the specified section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func numberOfItems(inSection section: Int) -> Int
```

## Parameters 

`section`  

The index of the section for which you want a count of the items.

## Return Value

The number of items in the specified section.

## See Also

### Getting the state of the collection view

var numberOfSections: Int

The number of sections displayed by the collection view.

var visibleCells: [UICollectionViewCell]

An array of visible cells currently displayed by the collection view.

