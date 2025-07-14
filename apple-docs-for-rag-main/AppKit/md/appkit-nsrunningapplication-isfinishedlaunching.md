

- AppKit
- NSRunningApplication
-  isFinishedLaunching 

Instance Property

# isFinishedLaunching

Indicates whether the receiver’s process has finished launching,

macOS 10.6+

``` source
var isFinishedLaunching: Bool { get }
```

## Discussion

The value of this property corresponds to the running application having received an didFinishLaunchingNotification notification internally. Some applications do not post this notification (applications that do not rely on NSApplication) and so are never reported as finished launching.

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

var processIdentifier: pid_t

Indicates the process identifier (pid) of the application.

var ownsMenuBar: Bool

Returns whether the application owns the current menu bar.

