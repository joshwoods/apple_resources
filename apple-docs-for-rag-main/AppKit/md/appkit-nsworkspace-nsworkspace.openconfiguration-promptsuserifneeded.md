

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  promptsUserIfNeeded 

Instance Property

# promptsUserIfNeeded

A Boolean value indicating whether to display errors, authentication requests, or other UI elements to the user.

macOS 10.15+

``` source
var promptsUserIfNeeded: Bool { get set }
```

## Discussion

When the value of this property is true, the system presents a user interface to request or display relevant information. The system waits until the user dismisses the UI before calling any relevant completion handlers. The default value of this property is true.

