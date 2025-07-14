

- AppKit
- NSCollectionViewFlowLayout
-  headerReferenceSize 

Instance Property

# headerReferenceSize

The default size to use for section headers.

macOS 10.11+

``` source
@MainActor
var headerReferenceSize: NSSize { get set }
```

## Discussion

If the delegate does not implement the collectionView(_:layout:referenceSizeForHeaderInSection:) method, the flow layout object uses the value of this property as the header size.

The layout object uses only the value that is appropriate for the current scrolling direction. In other words, the layout object uses only the height value when the content scrolls vertically, setting the width of the header to the width of the collection view. Similarly, the layout object uses only the width value when the content scrolls horizontally, setting the header’s height to the height of the collection view. If the size value for the appropriate dimension is `0`, the layout object omits the header entirely.

The default value of this property is NSZeroSize.

## See Also

### Configuring the Supplementary Views

var footerReferenceSize: NSSize

The default size to use for section footers.

