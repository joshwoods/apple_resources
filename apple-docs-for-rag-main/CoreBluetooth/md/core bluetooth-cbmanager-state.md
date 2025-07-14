

- Core Bluetooth
- CBManager
-  state 

Instance Property

# state

The current state of the manager.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var state: CBManagerState { get }
```

## Discussion

This state is initially set to CBManagerState.unknown. When the state updates, the manager calls its delegate’s centralManagerDidUpdateState(_:) method.

## See Also

### Accessing the Manager’s Properties

enum CBManagerState

The possible states of a Core Bluetooth manager.

