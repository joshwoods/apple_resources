

- XCUIAutomation
- XCUIApplication
-  activate() 

Instance Method

# activate()

Activates the application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func activate()
```

## Discussion

This call is synchronous. The application is in a state ready to handle events when this method returns.

If the application isn’t running prior to calling activate(), it launches automatically.

If the application previously launched via launch(), the system supplies the launch arguments and environment variables from the original call to launch() again.

Unlike launch(), a call to activate() doesn’t terminate the existing instance if the application is already running.

The system reports any failure in the activation or launch sequence as a test failure and the test is halted at that point.

