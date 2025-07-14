

- AppKit
- NSCell
-  action 

Instance Property

# action

The action performed by the cell.

macOS

``` source
@MainActor
var action: Selector? { get set }
```

## Discussion

The value of this property is the selector to call on the cell’s target object. Set the value of this property to `nil` to stop the delivery of action messages.

The default value of this property is `nil`. Setting the value of this property raises with internalInconsistencyException. Subclasses are expected to override this property as part of their target/action implementation.

## See Also

### Managing the Target and Action

var target: AnyObject?

The object that receives the cell’s action messages.

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

