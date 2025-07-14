

- AppKit
- NSApplication
-  isActive 

Instance Property

# isActive

A Boolean value indicating whether this is the active app.

macOS

``` source
@MainActor
var isActive: Bool { get }
```

## Discussion

The value of this property is true if the app is active or false if it’s not.

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

func deactivate()

Deactivates the receiver.

func yieldActivation(to: NSRunningApplication)

Explicitly allows another app to make itself active.

func yieldActivation(toApplicationWithBundleIdentifier: String)

Explicitly allows another app to make itself active.

struct ActivationOptions

The following flags are for activate(options:).

