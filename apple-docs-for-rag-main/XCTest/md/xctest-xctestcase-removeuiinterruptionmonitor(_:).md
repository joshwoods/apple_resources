

- XCTest
- XCTestCase
-  removeUIInterruptionMonitor(\_:) 

Instance Method

# removeUIInterruptionMonitor(\_:)

Removes a handler using the token from when you added the handler.

``` source
func removeUIInterruptionMonitor(_ monitor: any NSObjectProtocol)
```

## Parameters 

`monitor`  

An identifier token for an interruption monitor, obtained from a previous call to addUIInterruptionMonitor(withDescription:handler:).

## Mentioned in 

Handling UI Interruptions

## See Also

### Monitoring UI Interruptions

Handling UI Interruptions

Improve your UI test’s stability by handling interface changes that block the UI elements under test.

func addUIInterruptionMonitor(withDescription: String, handler: (XCUIElement) -> Bool) -> any NSObjectProtocol

Adds a handler to the current context.

