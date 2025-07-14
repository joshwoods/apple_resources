

- AppKit
- NSWorkspace
-  openFile(\_:) Deprecated

Instance Method

# openFile(\_:)

Opens the specified file specified using the default app associated with its type.

macOS 10.0–11.0Deprecated

``` source
func openFile(_ fullPath: String) -> Bool
```

Deprecated

Use open(_:) instead.

## Parameters 

`fullPath`  

The full path to the file.

## Return Value

true if the file was successfully opened; otherwise, false.

## Discussion

The sending app is deactivated before the request is sent.

It is safe to call this method from any thread in your app in macOS 10.6 and later.

## See Also

### Methods

func open(URL, options: NSWorkspace.LaunchOptions, configuration: [NSWorkspace.LaunchConfigurationKey : Any]) throws -> NSRunningApplicationDeprecated

func open([URL], withApplicationAt: URL, options: NSWorkspace.LaunchOptions, configuration: [NSWorkspace.LaunchConfigurationKey : Any]) throws -> NSRunningApplicationDeprecated

func openFile(String, withApplication: String?) -> Bool

Opens a file using the specified app.

Deprecated

func openFile(String, withApplication: String?, andDeactivate: Bool) -> Bool

Opens the specified file and optionally deactivates the sending app.

Deprecated

func openFile(String, from: NSImage?, at: NSPoint, in: NSView?) -> Bool

Opens a file using the default app for its type and animates the action using a custom icon.

Deprecated

func launchApplication(String) -> Bool

Launches the specified app.

Deprecated

func launchApplication(String, showIcon: Bool, autolaunch: Bool) -> Bool

Launches the specified app using additional options.

Deprecated

func launchApplication(at: URL, options: NSWorkspace.LaunchOptions, configuration: [NSWorkspace.LaunchConfigurationKey : Any]) throws -> NSRunningApplication

Launches the app at the specified URL.

Deprecated

func performFileOperation(NSWorkspace.FileOperationName, source: String, destination: String, files: [Any], tag: UnsafeMutablePointer&lt;Int>?) -> Bool

Performs a file operation on a set of files in a particular directory.

Deprecated

func fullPath(forApplication: String) -> String?

Returns the full path for the specified app.

Deprecated

func absolutePathForApplication(withBundleIdentifier: String) -> String?

Returns the absolute file system path of an app bundle.

Deprecated

func launchApplication(withBundleIdentifier: String, options: NSWorkspace.LaunchOptions, additionalEventParamDescriptor: NSAppleEventDescriptor?, launchIdentifier: AutoreleasingUnsafeMutablePointer&lt;NSNumber?>?) -> Bool

Launches the app corresponding to the specified `bundleIdentifier`.

Deprecated

func open([URL], withAppBundleIdentifier: String?, options: NSWorkspace.LaunchOptions, additionalEventParamDescriptor: NSAppleEventDescriptor?, launchIdentifiers: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> Bool

Opens one or more files from an array of URLs.

Deprecated

func mountedRemovableMedia() -> [Any]?

Returns the full pathnames of all currently mounted removable disks.

Deprecated

func mountedLocalVolumePaths() -> [Any]?

Returns the mount points of all local volumes, not just the removable ones returned by mountedRemovableMedia().

Deprecated

