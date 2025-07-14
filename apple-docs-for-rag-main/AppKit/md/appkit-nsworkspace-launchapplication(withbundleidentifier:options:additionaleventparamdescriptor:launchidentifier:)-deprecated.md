

- AppKit
- NSWorkspace
-  launchApplication(withBundleIdentifier:options:additionalEventParamDescriptor:launchIdentifier:) Deprecated

Instance Method

# launchApplication(withBundleIdentifier:options:additionalEventParamDescriptor:launchIdentifier:)

Launches the app corresponding to the specified `bundleIdentifier`.

macOS 10.0–11.0Deprecated

``` source
func launchApplication(
    withBundleIdentifier bundleIdentifier: String,
    options: NSWorkspace.LaunchOptions = [],
    additionalEventParamDescriptor descriptor: NSAppleEventDescriptor?,
    launchIdentifier identifier: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

Deprecated

Use openApplication(at:configuration:completionHandler:) instead.

## Parameters 

`bundleIdentifier`  

A bundle identifier string. This value corresponds to the value in the `CFBundleIdentifier` key of the app’s `Info.plist` file. For example, the bundle identifier of the TextEdit app is `com.apple.TextEdit`.

`options`  

Options to use when launching the app. Values for this parameter are described in NSWorkspace.LaunchOptions.

`descriptor`  

Additional options specified in an AppleEvent-style descriptor. For example, you could use this parameter to specify additional documents to open when the app is launched.

`identifier`  

The `launchIdentifiers` are currently unused, and you should pass `NULL`.

## Return Value

true if the app was found and launched; otherwise, false.

## Discussion

It is safe to call this method from any thread of your app.

## See Also

### Methods

func open(URL, options: NSWorkspace.LaunchOptions, configuration: [NSWorkspace.LaunchConfigurationKey : Any]) throws -> NSRunningApplicationDeprecated

func open([URL], withApplicationAt: URL, options: NSWorkspace.LaunchOptions, configuration: [NSWorkspace.LaunchConfigurationKey : Any]) throws -> NSRunningApplicationDeprecated

func openFile(String) -> Bool

Opens the specified file specified using the default app associated with its type.

Deprecated

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

func open([URL], withAppBundleIdentifier: String?, options: NSWorkspace.LaunchOptions, additionalEventParamDescriptor: NSAppleEventDescriptor?, launchIdentifiers: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> Bool

Opens one or more files from an array of URLs.

Deprecated

func mountedRemovableMedia() -> [Any]?

Returns the full pathnames of all currently mounted removable disks.

Deprecated

func mountedLocalVolumePaths() -> [Any]?

Returns the mount points of all local volumes, not just the removable ones returned by mountedRemovableMedia().

Deprecated

