

- AppKit
- NSCollectionViewLayoutAttributes
-  representedElementCategory 

Instance Property

# representedElementCategory

The type of the element.

macOS 10.11+

``` source
@MainActor
var representedElementCategory: NSCollectionElementCategory { get }
```

## Discussion

Use this property to distinguish whether the layout attributes apply to an item, a supplementary view, a decoration view, or another type of element presented by the collection view.

## See Also

### Identifying the Element

var indexPath: IndexPath?

The index path of the element.

var representedElementKind: String?

The identifier for specific elements of your collection view interface.

class let elementKindInterItemGapIndicator: String

The element kind string assigned to the attributes object when it represents an inter-item gap.

class let elementKindSectionFooter: String

A supplementary view that acts as a footer for a given section.

class let elementKindSectionHeader: String

A supplementary view that acts as a header for a given section.

