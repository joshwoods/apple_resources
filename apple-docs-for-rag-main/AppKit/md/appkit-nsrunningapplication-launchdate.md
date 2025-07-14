

- AppKit
- NSRunningApplication
-  launchDate 

Instance Property

# launchDate

Indicates the date when the application was launched.

macOS 10.6+

``` source
var launchDate: Date? { get }
```

## Discussion

This property is only available for applications that were launched by LaunchServices.

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

var isFinishedLaunching: Bool

Indicates whether the receiver’s process has finished launching,

var processIdentifier: pid_t

Indicates the process identifier (pid) of the application.

var ownsMenuBar: Bool

Returns whether the application owns the current menu bar.

