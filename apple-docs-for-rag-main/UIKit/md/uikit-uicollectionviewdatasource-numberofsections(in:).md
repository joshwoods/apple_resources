

- UIKit
- UICollectionViewDataSource
-  numberOfSections(in:) 

Instance Method

# numberOfSections(in:)

Asks your data source object for the number of sections in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func numberOfSections(in collectionView: UICollectionView) -> Int
```

## Parameters 

`collectionView`  

The collection view requesting this information.

## Return Value

The number of sections in `collectionView`.

## Discussion

If you don’t implement this method, the collection view uses a default value of 1.

## See Also

### Getting item and section metrics

func collectionView(UICollectionView, numberOfItemsInSection: Int) -> Int

Asks your data source object for the number of items in the specified section.

**Required**

