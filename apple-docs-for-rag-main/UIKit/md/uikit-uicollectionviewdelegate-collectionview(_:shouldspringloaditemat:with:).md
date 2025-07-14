

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:shouldSpringLoadItemAt:with:) 

Instance Method

# collectionView(\_:shouldSpringLoadItemAt:with:)

Determines whether the spring-loading interaction effect is displayed for the specified item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    shouldSpringLoadItemAt indexPath: IndexPath,
    with context: any UISpringLoadedInteractionContext
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object notifying you of the interaction.

`indexPath`  

The index path of the item for which the spring-loading behavior applies.

`context`  

A context object containing information about the item and view on which to display the spring-loading interaction.

## Return Value

true to apply the spring-loading behavior for the item or false to suppress the behavior altogether.

## Discussion

If you do not implement this method, the collection view assumes a return value of true.

