

- SwiftUI
- App
-  main() 

Type Method

# main()

Initializes and runs the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
static func main()
```

## Discussion

If you precede your App conformer’s declaration with the @main attribute, the system calls the conformer’s `main()` method to launch the app. SwiftUI provides a default implementation of the method that manages the launch process in a platform-appropriate way.

## See Also

### Running an app

init()

Creates an instance of the app using the body that you define for its content.

**Required**

