

- AppKit
- NSCollectionViewFlowLayout
-  footerReferenceSize 

Instance Property

# footerReferenceSize

The default size to use for section footers.

macOS 10.11+

``` source
@MainActor
var footerReferenceSize: NSSize { get set }
```

## Discussion

If the delegate does not implement the collectionView(_:layout:referenceSizeForFooterInSection:) method, the flow layout object uses the value of this property as the footer size.

The layout object uses only the value that is appropriate for the current scrolling direction. In other words, the layout object uses only the height value when the content scrolls vertically, setting the width of the footer to the width of the collection view. Similarly, the layout object uses only the width value when the content scrolls horizontally, setting the footer’s height to the height of the collection view. If the size value for the appropriate dimension is `0`, the layout object omits the footer entirely.

The default value of this property is NSZeroSize.

## See Also

### Configuring the Supplementary Views

var headerReferenceSize: NSSize

The default size to use for section headers.

