

- AppKit
- App and Environment
- NSWorkspace
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Overview

The table below describes keys for an `NSDictionary` object containing information about an app. This dictionary is returned by activeApplication() and launchedApplications, and is also provided in the `userInfo` of `NSWorkspace` notifications for app launch and termination.

Note that these constants are considered legacy.

Note

It is strongly suggested that you use the `NSWorkspace` class’s runningApplications method and the NSRunningApplication class to retrieve this information in apps target macOS 10.6 and later, rather than the activeApplication() and launchedApplications methods.

| Key | Value |
|----|----|
| `@"NSApplicationPath"` | The full path to the app, as a `NSString` object. |
| `@"NSApplicationName"` | The app’s name, as an `NSString` object. |
| `@"NSApplicationBundleIdentifier"` | The app’s bundle identifier, as an `NSString` object. |
| `@"NSApplicationProcessIdentifier"` | The app’s process ID, as an `NSNumber` object. |
| `@"NSApplicationProcessSerialNumberHigh"` | The high long of the process serial number (PSN), as an `NSNumber` object. |
| `@"NSApplicationProcessSerialNumberLow"` | The low long of the process serial number (PSN), as an `NSNumber` object. |

## Topics

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

func activeApplication() -> [AnyHashable : Any]?

Returns a dictionary with information about the current active app.

Deprecated

func icon(forFileType: String) -> NSImage

Returns an image containing the icon for files of the specified type.

Deprecated

### Types

struct LaunchOptions

Constants specifying how you want to launch an app

struct LaunchConfigurationKey

The following keys can be used in the configuration dictionary of the launchApplication(at:options:configuration:) method. Each key is optional, and if omitted, default behavior is applied.

Deprecated

struct FileOperationName

These constants specify different types of file operations used by performFileOperation(_:source:destination:files:tag:).

Deprecated

### Constants

class let applicationUserInfoKey: String

The value corresponding to this key is an instance of NSRunningApplication that reflects the affected app.

### Notifications

class let didPerformFileOperationNotification: NSNotification.Name

Posted when a file operation has been performed in the receiving app.

Deprecated

