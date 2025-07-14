

- XCUIAutomation
- XCUIApplication
-  launchEnvironment 

Instance Property

# launchEnvironment

The environment variables that pass to the application on launch.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var launchEnvironment: [String : String] { get set }
```

## Discussion

If not modified, these are the environment variables that Xcode passes to the application on launch. You can change, add to, or remove the environment variables. Unlike with Process, you can modify the environment variables after the application launches. Such changes don’t affect the current launch session, but do take effect the next time the application launches.

## See Also

### Launching the application

func launch()

Launches the application.

var launchArguments: [String]

The arguments that pass to the application on launch.

func open(URL)

Launches the application by URL.

