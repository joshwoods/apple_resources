

- AppKit
- NSCollectionLayoutDecorationItem
-  zIndex 

Instance Property

# zIndex

The vertical stacking order of the decoration item in relation to other items in the section.

macOS 10.15+

``` source
@MainActor
var zIndex: Int { get set }
```

## Discussion

The default value of this property is `0`, which means the decoration item appears below all other items in the section.

