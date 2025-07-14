

- XCTest
- XCTestCase
-  addUIInterruptionMonitor(withDescription:handler:) 

Instance Method

# addUIInterruptionMonitor(withDescription:handler:)

Adds a handler to the current context.

``` source
func addUIInterruptionMonitor(
    withDescription handlerDescription: String,
    handler: @escaping (XCUIElement) -> Bool
) -> any NSObjectProtocol
```

## Parameters 

`handlerDescription`  

An explanation of the behavior and purpose of this handler, mainly used for debugging and analysis.

`handler`  

A handler block for handling asynchronous UI interruptions such as alerts and other dialogs. Handlers should return true if they handled the UI, false if they did not. The handler is passed an XCUIElement representing the top level UI element for the alert.

## Return Value

Returns a token that can be used to unregister the handler. Handlers are invoked in the reverse order in which they are added until one of the handlers returns true, indicating that it has handled the alert.

## Mentioned in 

Handling UI Interruptions

## See Also

### Monitoring UI Interruptions

Handling UI Interruptions

Improve your UI test’s stability by handling interface changes that block the UI elements under test.

func removeUIInterruptionMonitor(any NSObjectProtocol)

Removes a handler using the token from when you added the handler.

