

- UIKit
- UIApplicationDelegate
-  main() 

Type Method

# main()

Provides the top-level entry point for the app.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor @preconcurrency
static func main()
```

## Discussion

UIApplicationDelegate provides an implementation of the main() method so that it can serve as the main entry point for a UIKit app. The system calls the main() method to launch your app; you never call it yourself. You can have exactly one entry point in your app, which you mark with the `@main` attribute.

