

- UIKit
- UIAccessibilityCustomRotor
-  UIAccessibilityCustomRotor.Direction 

Enumeration

# UIAccessibilityCustomRotor.Direction

Constants that indicate the search direction.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Direction
```

## Topics

### Constants

case previous

The previous search item.

case next

The next search item.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Navigating to the next item

var itemSearchBlock: UIAccessibilityCustomRotor.Search

The block for retrieving the next or previous rotor.

typealias Search

The block type for retrieving the next or previous rotor.

