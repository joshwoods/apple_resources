

- UIKit
- UICollectionViewDataSource
-  collectionView(\_:numberOfItemsInSection:) 

Instance Method

# collectionView(\_:numberOfItemsInSection:)

Asks your data source object for the number of items in the specified section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func collectionView(
    _ collectionView: UICollectionView,
    numberOfItemsInSection section: Int
) -> Int
```

**Required**

## Parameters 

`collectionView`  

The collection view requesting this information.

`section`  

An index number identifying a section in `collectionView`. This index value is 0-based.

## Return Value

The number of items in `section`.

## See Also

### Getting item and section metrics

func numberOfSections(in: UICollectionView) -> Int

Asks your data source object for the number of sections in the collection view.

