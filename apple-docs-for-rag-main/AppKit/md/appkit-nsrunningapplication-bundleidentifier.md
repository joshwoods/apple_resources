

- AppKit
- NSRunningApplication
-  bundleIdentifier 

Instance Property

# bundleIdentifier

Indicates the `CFBundleIdentifier` of the application.

macOS 10.6+

``` source
var bundleIdentifier: String? { get }
```

## Discussion

The value of this property will be `nil` if the application does not have an Info.plist.

## See Also

### Application information

var localizedName: String?

Indicates the localized name of the application.

var icon: NSImage?

Returns the icon for the receiver’s application.

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

var ownsMenuBar: Bool

Returns whether the application owns the current menu bar.

