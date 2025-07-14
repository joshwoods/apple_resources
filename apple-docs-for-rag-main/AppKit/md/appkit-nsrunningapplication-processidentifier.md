

- AppKit
- NSRunningApplication
-  processIdentifier 

Instance Property

# processIdentifier

Indicates the process identifier (pid) of the application.

macOS 10.6+

``` source
var processIdentifier: pid_t { get }
```

## Discussion

Not all applications have a pid. Applications without a pid return a value of -1.

Do not rely on this for comparing processes, instead compare NSRunningApplication instances using isEqual(_:).

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

var ownsMenuBar: Bool

Returns whether the application owns the current menu bar.

