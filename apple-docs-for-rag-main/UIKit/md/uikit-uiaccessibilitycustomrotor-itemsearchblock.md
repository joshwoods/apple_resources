

- UIKit
- UIAccessibilityCustomRotor
-  itemSearchBlock 

Instance Property

# itemSearchBlock

The block for retrieving the next or previous rotor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var itemSearchBlock: UIAccessibilityCustomRotor.Search { get set }
```

## Discussion

Your implementation of the block facilitates navigation from the current rotor to the next or previous rotor.

## See Also

### Navigating to the next item

typealias Search

The block type for retrieving the next or previous rotor.

enum Direction

Constants that indicate the search direction.

