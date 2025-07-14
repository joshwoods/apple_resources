

- AppKit
- NSCollectionViewLayoutAttributes
-  representedElementKind 

Instance Property

# representedElementKind

The identifier for specific elements of your collection view interface.

macOS 10.11+

``` source
@MainActor
var representedElementKind: String? { get }
```

## Discussion

For supplementary and decoration views, you use this string to distinguish between views in a given section. You also use this string to identify the intended purpose of the view in your collection view interface.

When the value of the representedElementCategory property is NSCollectionElementCategory.item, this property is `nil`.

## See Also

### Identifying the Element

var representedElementCategory: NSCollectionElementCategory

The type of the element.

var indexPath: IndexPath?

The index path of the element.

class let elementKindInterItemGapIndicator: String

The element kind string assigned to the attributes object when it represents an inter-item gap.

class let elementKindSectionFooter: String

A supplementary view that acts as a footer for a given section.

class let elementKindSectionHeader: String

A supplementary view that acts as a header for a given section.

