

- UIKit
- UIAccessibilityCustomRotor
-  UIAccessibilityCustomRotor.Search 

Type Alias

# UIAccessibilityCustomRotor.Search

The block type for retrieving the next or previous rotor.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
typealias Search = (UIAccessibilityCustomRotorSearchPredicate) -> UIAccessibilityCustomRotorItemResult?
```

## See Also

### Navigating to the next item

var itemSearchBlock: UIAccessibilityCustomRotor.Search

The block for retrieving the next or previous rotor.

enum Direction

Constants that indicate the search direction.

