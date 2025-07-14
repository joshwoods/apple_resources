

- AppKit
- NSCollectionViewDataSource
-  collectionView(\_:numberOfItemsInSection:) 

Instance Method

# collectionView(\_:numberOfItemsInSection:)

Asks your data source object to provide the number of items in the specified section.

macOS 10.11+

``` source
@MainActor
func collectionView(
    _ collectionView: NSCollectionView,
    numberOfItemsInSection section: Int
) -> Int
```

**Required**

## Parameters 

`collectionView`  

The collection view requesting the information.

`section`  

The index number of the section. Section indexes are zero based.

## Return Value

The number of items in the specified section.

## Discussion

All data source objects must implement this method. Your implementation should quickly return the number of items in the specified section.

Make sure the number of items you return is accurate. The collectionView(_:itemForRepresentedObjectAt:) method of your data source object must be able to provide a visual representation for each item in the section.

## See Also

### Getting the Number of Sections and Items

func numberOfSections(in: NSCollectionView) -> Int

Asks your data source object to provide the total number of sections.

