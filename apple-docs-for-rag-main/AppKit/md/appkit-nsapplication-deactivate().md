

- AppKit
- NSApplication
-  deactivate() 

Instance Method

# deactivate()

Deactivates the receiver.

macOS

``` source
@MainActor
func deactivate()
```

## Mentioned in 

Passing control from one app to another with cooperative activation

## Discussion

Normally, you shouldn’t invoke this method—AppKit is responsible for proper deactivation.

## See Also

### Related Documentation

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

### Activating and Deactivating the App

Passing control from one app to another with cooperative activation

Request focus for your app, and coordinate passing control from one app to another.

func activate()

Activates the receiver app, if appropriate.

var isActive: Bool

A Boolean value indicating whether this is the active app.

func yieldActivation(to: NSRunningApplication)

Explicitly allows another app to make itself active.

func yieldActivation(toApplicationWithBundleIdentifier: String)

Explicitly allows another app to make itself active.

struct ActivationOptions

The following flags are for activate(options:).

