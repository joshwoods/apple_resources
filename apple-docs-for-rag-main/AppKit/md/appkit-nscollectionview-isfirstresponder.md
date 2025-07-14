

- AppKit
- NSCollectionView
-  isFirstResponder 

Instance Property

# isFirstResponder

A Boolean value indicating whether the collection view is the first responder.

macOS 10.5+

``` source
@MainActor
var isFirstResponder: Bool { get }
```

## Discussion

The value of this property is true when the collection view is the first responder. This property is fully key-value observing compliant.

