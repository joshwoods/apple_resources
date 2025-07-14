

- SwiftUI
- NSViewRepresentableContext
-  environment 

Instance Property

# environment

Environment data that describes the current state of the system.

macOS 10.15+

``` source
@MainActor @preconcurrency
var environment: EnvironmentValues { get }
```

## Discussion

Use the environment values to configure the state of your view when creating or updating it.

