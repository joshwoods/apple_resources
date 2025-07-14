

- UIKit
- UICollectionViewFlowLayout
-  footerReferenceSize 

Instance Property

# footerReferenceSize

The default sizes to use for section footers.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var footerReferenceSize: CGSize { get set }
```

## Discussion

If the delegate does not implement the collectionView(_:layout:referenceSizeForFooterInSection:) method, the flow layout object uses the default footer sizes set for this property.

During layout, only the size that corresponds to the appropriate scrolling direction is used. For example, for the vertical scrolling direction, the layout object uses the height value specified by this property. (In that instance, the width of the footer would be set to the width of the collection view.) If the size in the appropriate scrolling dimension is 0, no footer is added.

The default size values are (0, 0).

## See Also

### Related Documentation

var sectionInset: UIEdgeInsets

The margins used to lay out content in a section.

### Configuring headers and footers

var headerReferenceSize: CGSize

The default sizes to use for section headers.

Flow layout supplementary views

Constants that specify the types of supplementary views that can be presented using a flow layout.

