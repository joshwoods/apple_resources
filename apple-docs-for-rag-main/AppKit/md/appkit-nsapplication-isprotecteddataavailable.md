

- AppKit
- NSApplication
-  isProtectedDataAvailable 

Instance Property

# isProtectedDataAvailable

macOS 12.0+

``` source
@MainActor
var isProtectedDataAvailable: Bool { get }
```

## See Also

### Restoring App Windows at Launch

func extendStateRestoration()

Allows an app to extend its state restoration period.

func completeStateRestoration()

Completes the extended state restoration.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void) -> Bool

Invoked to request that a window be restored.

