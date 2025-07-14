

- AppKit
- NSCollectionViewDelegateFlowLayout
-  collectionView(\_:layout:minimumLineSpacingForSectionAt:) 

Instance Method

# collectionView(\_:layout:minimumLineSpacingForSectionAt:)

Asks the delegate for the spacing between successive rows or columns of a section.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    layout collectionViewLayout: NSCollectionViewLayout,
    minimumLineSpacingForSectionAt section: Int
) -> CGFloat
```

## Parameters 

`collectionView`  

The collection view object displaying the flow layout.

`collectionViewLayout`  

The layout object requesting the information.

`section`  

The index of the section whose line spacing is needed.

## Return Value

The minimum space (in points) to apply between successive lines in a section.

## Discussion

Implement this method when you want to provide custom line spacing for sections in the flow layout. Your implementation can return the same line spacing for all sections or it can return different line spacing for different sections. You can also adjust the line spacing of each section dynamically each time you update the layout. If you do not implement this method, the line spacing is obtained from the properties of the flow layout object.

For a vertically scrolling layout, this value represents the minimum spacing between successive rows. For a horizontally scrolling layout, this value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header and the first line or between the last line and the footer. For more information about how line spacing is applied, see the description of the minimumLineSpacing property.

## See Also

### Related Documentation

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

### Getting the Section Spacing

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, insetForSectionAt: Int) -> NSEdgeInsets

Asks the delegate for the margins to apply to content in the specified section.

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, minimumInteritemSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive items of a single row or column.

