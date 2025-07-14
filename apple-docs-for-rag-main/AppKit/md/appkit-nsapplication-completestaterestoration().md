

- AppKit
- NSApplication
-  completeStateRestoration() 

Instance Method

# completeStateRestoration()

Completes the extended state restoration.

macOS 10.7+

``` source
@MainActor
func completeStateRestoration()
```

## Discussion

This method informs the app that the extended state restoration is completed for the balancing .

If a window has some state that may take a long time to restore, such as a web page, you may use this method and methods to `completeStateRestoration` to extend the period of this crash protection beyond the default.

You call extendStateRestoration() within your implementation of restoreWindow(withIdentifier:state:completionHandler:). You would then call `completeStateRestoration` some time after the window is fully restored. If the app crashes in the interim, then it may offer to discard restorable state on the next launch.

The extendStateRestoration() and `completeStateRestoration` method act as a counter. Each call to extendStateRestoration()increments the counter, and must be matched with a corresponding call to `completeStateRestoration` which decrements it. When the counter reaches zero, the app is considered to have been fully restored, and any further calls are silently ignored.

This method is thread safe.

## See Also

### Restoring App Windows at Launch

var isProtectedDataAvailable: Bool

func extendStateRestoration()

Allows an app to extend its state restoration period.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void) -> Bool

Invoked to request that a window be restored.

