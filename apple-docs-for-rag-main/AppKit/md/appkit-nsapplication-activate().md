

- AppKit
- NSApplication
-  activate() 

Instance Method

# activate()

Activates the receiver app, if appropriate.

macOS 14.0+

``` source
@MainActor
func activate()
```

## Mentioned in 

Passing control from one app to another with cooperative activation

## Discussion

Use this method to request app activation; calling this method doesn’t guarantee app activation. For cooperative activation, the other app should call yieldActivation(to:) or equivalent before the target app invokes activate().

Invoking activate() on an already-active application cancels any pending activation yields by the receiver.

## See Also

### Activating and Deactivating the App

Passing control from one app to another with cooperative activation

Request focus for your app, and coordinate passing control from one app to another.

func deactivate()

Deactivates the receiver.

var isActive: Bool

A Boolean value indicating whether this is the active app.

func yieldActivation(to: NSRunningApplication)

Explicitly allows another app to make itself active.

func yieldActivation(toApplicationWithBundleIdentifier: String)

Explicitly allows another app to make itself active.

struct ActivationOptions

The following flags are for activate(options:).

