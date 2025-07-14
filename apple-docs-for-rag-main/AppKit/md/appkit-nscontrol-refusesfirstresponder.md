

- AppKit
- NSControl
-  refusesFirstResponder 

Instance Property

# refusesFirstResponder

A Boolean value indicating whether the receiver refuses the first responder role.

macOS

``` source
@MainActor
var refusesFirstResponder: Bool { get set }
```

## Discussion

The value of this property is true if the receiver refuses the first responder role; otherwise, false.

## See Also

### Related Documentation

var objectValue: Any?

The value of the receiver’s cell as an Objective-C object.

var doubleValue: Double

The value of the receiver’s cell as a double-precision floating-point number.

var floatValue: Float

The value of the receiver’s cell as a single-precision floating-point number.

### Activating from the Keyboard

func performClick(Any?)

Simulates a single mouse click on the receiver.

