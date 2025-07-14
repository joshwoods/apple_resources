

- UIKit
- UICollectionViewDelegateFlowLayout
-  collectionView(\_:layout:minimumLineSpacingForSectionAt:) 

Instance Method

# collectionView(\_:layout:minimumLineSpacingForSectionAt:)

Asks the delegate for the spacing between successive rows or columns of a section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    layout collectionViewLayout: UICollectionViewLayout,
    minimumLineSpacingForSectionAt section: Int
) -> CGFloat
```

## Parameters 

`collectionView`  

The collection view object displaying the flow layout.

`collectionViewLayout`  

The layout object requesting the information.

`section`  

The index number of the section whose line spacing is needed.

## Return Value

The minimum space (measured in points) to apply between successive lines in a section.

## Discussion

If you do not implement this method, the flow layout uses the value in its minimumLineSpacing property to set the space between lines instead. Your implementation of this method can return a fixed value or return different spacing values for each section.

For a vertically scrolling grid, this value represents the minimum spacing between successive rows. For a horizontally scrolling grid, this value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header and the first line or between the last line and the footer.

## See Also

### Getting the section spacing

func collectionView(UICollectionView, layout: UICollectionViewLayout, insetForSectionAt: Int) -> UIEdgeInsets

Asks the delegate for the margins to apply to content in the specified section.

func collectionView(UICollectionView, layout: UICollectionViewLayout, minimumInteritemSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive items in the rows or columns of a section.

