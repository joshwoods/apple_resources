

- XCUIAutomation
- XCUIApplication
-  launchArguments 

Instance Property

# launchArguments

The arguments that pass to the application on launch.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var launchArguments: [String] { get set }
```

## Discussion

If not modified, these are the arguments that Xcode passes to the application on launch. You can change, add to, or remove the arguments. Unlike with Process, you can also modify these arguments after the application launches. Such changes don’t affect the current launch session, but do take effect the next time the application launches.

## See Also

### Launching the application

func launch()

Launches the application.

var launchEnvironment: [String : String]

The environment variables that pass to the application on launch.

func open(URL)

Launches the application by URL.

