

- AppKit
- NSAccessibilityCustomRotor
-  init(rotorType:itemSearchDelegate:) 

Initializer

# init(rotorType:itemSearchDelegate:)

Creates a custom rotor with the specified rotor type and item search delegate.

macOS 10.13+

``` source
init(
    rotorType: NSAccessibilityCustomRotor.RotorType,
    itemSearchDelegate: any NSAccessibilityCustomRotorItemSearchDelegate
)
```

## See Also

### Creating a Rotor

init(label: String, itemSearchDelegate: any NSAccessibilityCustomRotorItemSearchDelegate)

Creates a custom rotor with the specified label and item search delegate.

