

- AppKit
- NSCollectionViewDataSource
-  numberOfSections(in:) 

Instance Method

# numberOfSections(in:)

Asks your data source object to provide the total number of sections.

macOS 10.11+

``` source
@MainActor
optional func numberOfSections(in collectionView: NSCollectionView) -> Int
```

## Parameters 

`collectionView`  

The collection view requesting the information.

## Return Value

The number of sections in the specified collection view.

## Discussion

Implement this method when the organization of your data requires more than one section. If you do not implement this method, the collection view creates only one section.

## See Also

### Getting the Number of Sections and Items

func collectionView(NSCollectionView, numberOfItemsInSection: Int) -> Int

Asks your data source object to provide the number of items in the specified section.

**Required**

