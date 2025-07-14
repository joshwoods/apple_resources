

- AppKit
- NSApplication
-  yieldActivation(toApplicationWithBundleIdentifier:) 

Instance Method

# yieldActivation(toApplicationWithBundleIdentifier:)

Explicitly allows another app to make itself active.

macOS 14.0+

``` source
@MainActor
func yieldActivation(toApplicationWithBundleIdentifier bundleIdentifier: String)
```

## Parameters 

`bundleIdentifier`  

The bundle identifier to yield activation state to.

## Mentioned in 

Passing control from one app to another with cooperative activation

## Discussion

Calling this method doesn’t deactivate the yielding app, nor does it activate the app you yield to. For cooperative activation, the other app must request activation in the future by calling activate() or equivalent.

Use this method to yield activation to apps that aren’t running at the time the method invokes. If it’s known that the target application is running, use yieldActivation(to:) instead.

## See Also

### Activating and Deactivating the App

Passing control from one app to another with cooperative activation

Request focus for your app, and coordinate passing control from one app to another.

func activate()

Activates the receiver app, if appropriate.

func deactivate()

Deactivates the receiver.

var isActive: Bool

A Boolean value indicating whether this is the active app.

func yieldActivation(to: NSRunningApplication)

Explicitly allows another app to make itself active.

struct ActivationOptions

The following flags are for activate(options:).

