

- XCUIAutomation
- XCUIApplication
-  wait(for:timeout:) 

Instance Method

# wait(for:timeout:)

Waits for the application to reach the specified state or timeout.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func wait(
    for state: XCUIApplication.State,
    timeout: TimeInterval
) -> Bool
```

## Parameters 

`state`  

The requested application state.

`timeout`  

The amount of time to wait, in seconds, for the application to reach the requested application state.

## Return Value

A Boolean value that indicates whether the app is in the specified state, or can reach the specified state before the timeout.

