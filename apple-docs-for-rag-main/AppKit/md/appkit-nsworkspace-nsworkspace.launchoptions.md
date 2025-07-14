

- AppKit
- NSWorkspace
-  NSWorkspace.LaunchOptions 

Structure

# NSWorkspace.LaunchOptions

Constants specifying how you want to launch an app

macOS

``` source
struct LaunchOptions
```

## Topics

### Options

static var andPrint: NSWorkspace.LaunchOptions

Print items instead of opening them.

Deprecated

static var withErrorPresentation: NSWorkspace.LaunchOptions

Display an error panel to the user if a failure occurs.

Deprecated

static var inhibitingBackgroundOnly: NSWorkspace.LaunchOptions

Causes launch to fail if the target is background-only.

Deprecated

static var withoutAddingToRecents: NSWorkspace.LaunchOptions

Do not add the app or documents to the Recents menu.

Deprecated

static var withoutActivation: NSWorkspace.LaunchOptions

Launch the app but do not bring it into the foreground.

Deprecated

static var async: NSWorkspace.LaunchOptions

Launch the app and return the results asynchronously.

Deprecated

static var allowingClassicStartup: NSWorkspace.LaunchOptions

Start up the Classic compatibility environment, if it is required by the app.

Deprecated

static var preferringClassic: NSWorkspace.LaunchOptions

Force the app to launch in the Classic compatibility environment.

Deprecated

static var newInstance: NSWorkspace.LaunchOptions

Create a new instance of the app, even if one is already running.

Deprecated

static var andHide: NSWorkspace.LaunchOptions

Tell the app to hide itself as soon as it finishes launching.

Deprecated

static var andHideOthers: NSWorkspace.LaunchOptions

Hide all apps except the newly launched one.

Deprecated

static var `default`: NSWorkspace.LaunchOptions

Launch the app asynchronously and launch it in the Classic environment, if required.

Deprecated

### Initializers

init(rawValue: UInt)

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

### Types

struct LaunchConfigurationKey

The following keys can be used in the configuration dictionary of the launchApplication(at:options:configuration:) method. Each key is optional, and if omitted, default behavior is applied.

Deprecated

struct FileOperationName

These constants specify different types of file operations used by performFileOperation(_:source:destination:files:tag:).

Deprecated

