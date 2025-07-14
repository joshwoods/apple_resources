

- TVUIKit
- TVCollectionViewDelegateFullScreenLayout
-  collectionView(\_:layout:didCenterCellAt:) 

Instance Method

# collectionView(\_:layout:didCenterCellAt:)

Tells the delegate when a cell has completed the transition and has become the center cell.

tvOS 13.0+

``` source
optional func collectionView(
    _ collectionView: UICollectionView,
    layout collectionViewLayout: UICollectionViewLayout,
    didCenterCellAt indexPath: IndexPath
)
```

## See Also

### Managing Cell Transitions

func collectionView(UICollectionView, layout: UICollectionViewLayout, willCenterCellAt: IndexPath)

Tells the delegate when a cell is to be the center cell.

