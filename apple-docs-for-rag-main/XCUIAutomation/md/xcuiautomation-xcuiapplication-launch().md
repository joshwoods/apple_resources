

- XCUIAutomation
- XCUIApplication
-  launch() 

Instance Method

# launch()

Launches the application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func launch()
```

## Discussion

This call is synchronous. When it returns, the application launches and is ready to handle user events. The system reports any failure in the launch sequence as a test failure and halts the test at this point.

If the application is already running, this call terminates the existing instance, to ensure a clean launch state for the newly launched instance.

## See Also

### Launching the application

var launchArguments: [String]

The arguments that pass to the application on launch.

var launchEnvironment: [String : String]

The environment variables that pass to the application on launch.

func open(URL)

Launches the application by URL.

