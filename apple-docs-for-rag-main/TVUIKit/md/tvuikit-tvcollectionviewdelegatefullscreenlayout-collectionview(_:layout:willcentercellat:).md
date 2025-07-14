

- TVUIKit
- TVCollectionViewDelegateFullScreenLayout
-  collectionView(\_:layout:willCenterCellAt:) 

Instance Method

# collectionView(\_:layout:willCenterCellAt:)

Tells the delegate when a cell is to be the center cell.

tvOS 13.0+

``` source
optional func collectionView(
    _ collectionView: UICollectionView,
    layout collectionViewLayout: UICollectionViewLayout,
    willCenterCellAt indexPath: IndexPath
)
```

## See Also

### Managing Cell Transitions

func collectionView(UICollectionView, layout: UICollectionViewLayout, didCenterCellAt: IndexPath)

Tells the delegate when a cell has completed the transition and has become the center cell.

