

- AppKit
- NSWorkspace
-  NSWorkspace.LaunchConfigurationKey Deprecated

Structure

# NSWorkspace.LaunchConfigurationKey

The following keys can be used in the configuration dictionary of the launchApplication(at:options:configuration:) method. Each key is optional, and if omitted, default behavior is applied.

macOS 10.6–11.0Deprecated

``` source
struct LaunchConfigurationKey
```

Deprecated

Use NSWorkspace.OpenConfiguration instead.

## Topics

### Type Properties

static let appleEvent: NSWorkspace.LaunchConfigurationKey

The value is the first NSAppleEventDescriptor to send to the new app. If an instance of the app is already running, this is sent to that app.

static let architecture: NSWorkspace.LaunchConfigurationKey

The value is an NSNumber containing an Mach-O Architecture constant. Ignored if a new instance of the app is not launched.

static let arguments: NSWorkspace.LaunchConfigurationKey

The value is an `NSArray` of `NSStrings`, passed to the new app in the `argv` parameter. Ignored if a new instance of the app is not launched. This constant is not available to sandboxed apps.

static let environment: NSWorkspace.LaunchConfigurationKey

The value is an `NSDictionary`, mapping `NSStrings` to `NSStrings`, containing environment variables to set for the new app. Ignored if a new instance of the app is not launched. This constant is not available to sandboxed apps.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Types

struct LaunchOptions

Constants specifying how you want to launch an app

struct FileOperationName

These constants specify different types of file operations used by performFileOperation(_:source:destination:files:tag:).

Deprecated

