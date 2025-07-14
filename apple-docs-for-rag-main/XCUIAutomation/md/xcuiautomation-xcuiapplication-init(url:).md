

- XCUIAutomation
- XCUIApplication
-  init(url:) 

Initializer

# init(url:)

Creates a proxy for the application at the specified file system URL.

macOSXcode 16.3+

``` source
@MainActor
init(url: URL)
```

## Discussion

This initializer is only available on macOS.

## See Also

### Creating an application proxy

init()

Creates a proxy for the application that’s configured as the Target Application in Xcode’s target settings.

init(bundleIdentifier: String)

Creates a proxy for an application for the specified bundle identifier.

