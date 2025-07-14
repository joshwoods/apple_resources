

- UIKit
- UICollectionViewDataSource
-  collectionView(\_:indexPathForIndexTitle:at:) 

Instance Method

# collectionView(\_:indexPathForIndexTitle:at:)

Asks the data source to return the index path of a collection view item that corresponds to one of your index entries.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 10.2+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    indexPathForIndexTitle title: String,
    at index: Int
) -> IndexPath
```

## Parameters 

`collectionView`  

The collection view requesting this information.

`title`  

The title of the index item. This string corresponds to one of the strings you returned in your indexTitles(for:) method.

`index`  

The index into the array returned by the indexTitles(for:) method that corresponds to the index title.

## Return Value

The index path for the collection view item that should appear when the user selects the index.

## Discussion

Use this method to support fast scrolling through your collection view’s content. After returning a set of index strings from your indexTitles(for:) method, the collection view calls this method for each string to fetch the collection view item to use as the scrolling destination.

## See Also

### Configuring an index

func indexTitles(for: UICollectionView) -> [String]?

Asks the data source to return the titles for the index items to display for the collection view.

