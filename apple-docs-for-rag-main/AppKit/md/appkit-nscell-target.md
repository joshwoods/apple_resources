

- AppKit
- NSCell
-  target 

Instance Property

# target

The object that receives the cell’s action messages.

macOS

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## Discussion

The value of this property is the object that implements the selector specified by the action property. Set the value of this property to `nil` to stop the delivery of action messages.

The default value of this property is `nil`. Setting the value of this property raises with internalInconsistencyException. Subclasses are expected to override this property as part of their target/action implementation.

## See Also

### Managing the Target and Action

var action: Selector?

The action performed by the cell.

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the receiver sends action messages to its target.

