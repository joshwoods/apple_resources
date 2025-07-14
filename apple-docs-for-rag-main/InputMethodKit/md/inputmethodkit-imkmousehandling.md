

- InputMethodKit
-  IMKMouseHandling 

Protocol

# IMKMouseHandling

The `IMKMouseHandling` protocol defines methods that your input method can implement to handle mouse events.

macOS 10.5+

``` source
protocol IMKMouseHandling
```

## Topics

### Handling Mouse Events

func mouseDown(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, continueTracking: UnsafeMutablePointer&lt;ObjCBool>!, client: Any!) -> Bool

Handles mouse-down event send to an input method.

**Required**

func mouseUp(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, client: Any!) -> Bool

Handles a mouse-up event sent to an input method.

**Required**

func mouseMoved(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, client: Any!) -> Bool

Handles a mouse-moved event sent to an input method.

**Required**

## Relationships

### Conforming Types

- IMKInputController

## See Also

### Protocols

IMKServerInput

`IMKServerInput` is an informal protocol that defines methods for receiving text events. This is intentionally not a formal protocol because there are three ways to receive events. An input method chooses one of the following approaches and implements the appropriate methods:

protocol IMKStateSetting

The `IMKStateSetting` protocol defines methods for setting or accessing values that indicate the state of an input method.

