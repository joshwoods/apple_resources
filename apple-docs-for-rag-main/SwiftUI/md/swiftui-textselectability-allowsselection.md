

- SwiftUI
- TextSelectability
-  allowsSelection 

Type Property

# allowsSelection

A Boolean value that indicates whether the selectability type allows selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static var allowsSelection: Bool { get }
```

**Required**

## Discussion

Conforming types, such as EnabledTextSelectability and DisabledTextSelectability, return `true` or `false` for this property as appropriate. SwiftUI expects this value for a given selectability type to be constant, unaffected by global state.

