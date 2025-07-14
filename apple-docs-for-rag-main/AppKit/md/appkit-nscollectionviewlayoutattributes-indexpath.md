

- AppKit
- NSCollectionViewLayoutAttributes
-  indexPath 

Instance Property

# indexPath

The index path of the element.

macOS 10.11+

``` source
@MainActor
var indexPath: IndexPath? { get set }
```

## Discussion

Use the index path to locate information about the item in your app’s data structures. For supplementary and decoration views, you must also use the representedElementKind property to identify the element.

## See Also

### Identifying the Element

var representedElementCategory: NSCollectionElementCategory

The type of the element.

var representedElementKind: String?

The identifier for specific elements of your collection view interface.

class let elementKindInterItemGapIndicator: String

The element kind string assigned to the attributes object when it represents an inter-item gap.

class let elementKindSectionFooter: String

A supplementary view that acts as a footer for a given section.

class let elementKindSectionHeader: String

A supplementary view that acts as a header for a given section.

