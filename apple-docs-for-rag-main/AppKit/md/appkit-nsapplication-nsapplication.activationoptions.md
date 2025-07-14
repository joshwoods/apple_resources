

- AppKit
- NSApplication
-  NSApplication.ActivationOptions 

Structure

# NSApplication.ActivationOptions

The following flags are for activate(options:).

macOS

``` source
struct ActivationOptions
```

## Topics

### Options

static var activateAllWindows: NSApplication.ActivationOptions

By default, activation brings only the main and key windows forward. If you specify NSApplicationActivateAllWindows, all of the application’s windows are brought forward.

### Initializers

init(rawValue: UInt)

Initializes a new activation options structure.

### Deprecated

static var activateIgnoringOtherApps: NSApplication.ActivationOptions

The application is activated regardless of the currently active app.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

func yieldActivation(toApplicationWithBundleIdentifier: String)

Explicitly allows another app to make itself active.

