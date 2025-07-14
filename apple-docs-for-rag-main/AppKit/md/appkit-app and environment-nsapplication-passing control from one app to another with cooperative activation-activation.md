

- AppKit
- App and Environment
- NSApplication
-  Passing control from one app to another with cooperative activation 

Article

# Passing control from one app to another with cooperative activation

Request focus for your app, and coordinate passing control from one app to another.

## Overview

When someone uses your app and another app unexpectedly steals focus, the user experience can be compromised. Not only is it inconvenient for people to switch back to their original app, if they’re typing when the switch occurs, they might accidentally enter text into the wrong app, inadvertently disclosing sensitive information.

Cooperative activation addresses this problem by making app activation a request instead of a command. Instead of apps stealing focus, they now request focus from the system when they’re ready. This means apps should set expectations accordingly when requesting activation and not assume the system will grant them activation. The system dynamically determines whether to grant activation state based on the context. This lets you request focus for your app when needed, and hand off focus from one app to another.

Related sessions from WWDC23

Session 10054: What’s new in AppKit

### Request activation to gain focus

When your app needs focus, call activate() on your app’s shared instance, or its shorthand version `NSApp`:

- Swift
- Objective-C

```
// Call this function when you want your app to request activation for itself.
NSApp.activate()
```

```
// Call this function when you want your app to request activation for itself.
[NSApp activate];
```

Calling this function sends a message to the system requesting activation for the app. Requesting activation doesn’t guarantee your app gains focus. People ultimately decide which apps gain focus by activating them through their device’s user interface. But if, after considering the user’s intent and larger system context, the system honors your app’s request, your app activates.

### Transfer control from one app to another by yielding and then activating

Passing control from one app to another is a two-step process.

1.  First yield from the currently running active app to the target app that you want to gain focus.

2.  Then activate the target app when it’s ready.

Only the active app can influence the activation context. It does so by yielding to an explicit target app before the target app activates. Then, when the target app requests activation, the system uses the yield as part of the context when making its decision. If the system honors the request, the active app deactivates, and the target app activates. Otherwise, the active app remains active. NSWorkspace automatically handles this for you when opening URLs or applications.

For example, to pass control from your active app to another target app (such as TextEdit, which is a good test candidate because it comes installed on every Mac):

1.  Get an instance of the target app you want to pass control to by calling runningApplications(withBundleIdentifier:), passing in the bundle identifier of the target app.

2.  Yield to the target app by calling yieldActivation(to:), passing the target app instance.

3.  Then activate the target by calling activate() on the target app instance.

- Swift
- Objective-C

```
// When you want to pass control to another application.

// Get an instance of the app you want to activate.
if let targetApp = NSRunningApplication.runningApplications(withBundleIdentifier:
                                                                "com.apple.TextEdit").first {
    // Yield to it.
    NSApp.yieldActivation(to:targetApp)

    // Then activate it.
    targetApp.activate()
}
```

```
// When you want to pass control from your app to another.

// Get an instance to the app you want to activate.
NSArray *targetApps = [NSRunningApplication runningApplicationsWithBundleIdentifier:@"com.apple.TextEdit"];
NSRunningApplication *targetApp = [targetApps firstObject];

if (targetApp != nil) {
    // Yield to it.
    [NSApp yieldActivationToApplication: targetApp];

    // Then activate it.
    [targetApp activateWithOptions:0];
}
```

Alternatively, if the app you want to pass control to isn’t currently running, call yieldActivation(toApplicationWithBundleIdentifier:) on the `NSApp` instance, passing in the bundle identifier of the target app you want to activate.

- Swift
- Objective-C

```
// Call this function from the active process.
// Yield to the app using the app's bundleIdentifier.
NSApp.yieldActivation(toApplicationWithBundleIdentifier: "com.example.targetApp")
```

```
// Call this function from the active process.
// Yield to the app using the app's bundleIdentifier.
[NSApp yieldActivationToApplicationWithBundleIdentifier: @"com.example.targetApp"];
```

Then call activate() on the target app when it’s ready to gain focus.

- Swift
- Objective-C

```
// Call this function from the target process.
// Have the app activate itself when it's ready.
NSApp.activate()
```

```
// Call this function from the target process.
// Have the app activate itself when it's ready.
[NSApp activate];
```

Choosing between NSRunningApplication or NSApplication for activation depends on which app you want to initiate the activation. Use `NSRunningApplication` if you want the active app to control when the target app activates. Use `NSApplication` (or `NSApp`) if you want the target app to activate itself.

### Replace calls to deactivate

When you call yieldActivation(to:), there’s no need to call deactivate() on the app losing focus. Cooperative activation APIs cause the receiver to draw inactive when another app activates. This is typically the behavior you want.

Replace calls to deactivate() with yieldActivation(to:) or equivalent. There’s also no need to call `deactivate()` if an app is hidden by calling hide(). The system implies deactivation when the app hides.

## See Also

### Activating and Deactivating the App

func activate()

Activates the receiver app, if appropriate.

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

