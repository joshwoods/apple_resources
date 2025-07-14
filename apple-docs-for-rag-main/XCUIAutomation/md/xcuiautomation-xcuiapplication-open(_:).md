

- XCUIAutomation
- XCUIApplication
-  open(\_:) 

Instance Method

# open(\_:)

Launches the application by URL.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+Xcode 16.3+

``` source
@MainActor
func open(_ url: URL)
```

## Parameters 

`url`  

The URL of the item to open the application to.

## See Also

### Launching the application

func launch()

Launches the application.

var launchArguments: [String]

The arguments that pass to the application on launch.

var launchEnvironment: [String : String]

The environment variables that pass to the application on launch.

