

- AppKit
- NSRunningApplication
-  ownsMenuBar 

Instance Property

# ownsMenuBar

Returns whether the application owns the current menu bar.

macOS 10.7+

``` source
var ownsMenuBar: Bool { get }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Application information

var localizedName: String?

Indicates the localized name of the application.

var icon: NSImage?

Returns the icon for the receiver’s application.

var bundleIdentifier: String?

Indicates the `CFBundleIdentifier` of the application.

var bundleURL: URL?

Indicates the URL to the application’s bundle.

var executableArchitecture: Int

Indicates the executing processor architecture for the application.

var executableURL: URL?

Indicates the URL to the application’s executable.

var launchDate: Date?

Indicates the date when the application was launched.

var isFinishedLaunching: Bool

Indicates whether the receiver’s process has finished launching,

var processIdentifier: pid_t

Indicates the process identifier (pid) of the application.

