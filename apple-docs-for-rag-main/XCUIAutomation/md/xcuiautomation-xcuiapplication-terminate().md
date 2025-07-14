

- XCUIAutomation
- XCUIApplication
-  terminate() 

Instance Method

# terminate()

Terminates any running instance of the application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func terminate()
```

## Discussion

If the application has an existing debug session via Xcode, the debugger sends a command to terminate the application. Otherwise, an appropriate platform-specific mechanism terminates the process.

