

- XCUIAutomation
- XCUIApplication
-  state 

Instance Property

# state

The most recent state of the application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var state: XCUIApplication.State { get }
```

## Discussion

The system monitors the app to update this property as the app’s state changes. Consequently, the system updates the value of this property asynchronously.

The system makes the following guarantees:

- When launch() and activate() return successfully, the state of the application is XCUIApplication.State.runningForeground. An exception to this is launching or activating a macOS agent application with LSUIElement set in its `Info.plist `file. This kind of application never gains foreground status and its state is XCUIApplication.State.runningBackground instead.

- When terminate() returns successfully, the state of the application is XCUIApplication.State.notRunning.

## See Also

### Determining application state

enum State

The possible states of an application during UI testing.

