

- AppKit
-  NSWorkspace 

Class

# NSWorkspace

A workspace that can launch other apps and perform a variety of file-handling services.

macOS

``` source
class NSWorkspace
```

## Mentioned in 

Passing control from one app to another with cooperative activation

## Overview

There is one shared NSWorkspace object per app. You use the class method shared to access it. For example, the following statement uses an NSWorkspace object to request that a file be opened in the TextEdit app:

- Swift
- Objective-C

```
NSWorkspace.shared.openFile("/Myfiles/README", withApplication: "TextEdit")
```

```
[[NSWorkspace sharedWorkspace] openFile:@"/Myfiles/README" withApplication:@"TextEdit"];
```

You can use the workspace object to:

- Open, manipulate, and get information about files and devices.

- Track changes to the file system, devices, and the user database.

- Get and set Finder information for files.

- Launch apps.

## Topics

### Accessing the Shared Workspace

class var shared: NSWorkspace

The shared workspace object.

### Accessing the Workspace Notification Center

var notificationCenter: NotificationCenter

The notification center for workspace notifications.

### Opening URLs

func open(URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens a URL asynchronously using the provided options.

func open([URL], withApplicationAt: URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Opens one or more URLs asynchronously in the specified app using the provided options.

func open(URL) -> Bool

Opens the location at the specified URL.

### Launching and Hiding Apps

func openApplication(at: URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Launches the app at the specified URL and asynchronously reports back on the app’s status.

func hideOtherApplications()

Hides all applications other than the sender.

### Managing Open Configurations

class OpenConfiguration

The configuration options for opening URLs or launching apps.

### Manipulating Files

func duplicate([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Duplicates the specified URLS asynchronously in the same manner as the Finder.

func recycle([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Moves the specified URLs to the trash in the same manner as the Finder.

func activateFileViewerSelecting([URL])

Activates the Finder, and opens one or more windows selecting the specified files.

func selectFile(String?, inFileViewerRootedAtPath: String) -> Bool

Selects the file at the specified path.

### Manipulating Uniform Type Identifier Information

func type(ofFile: String) throws -> String

Returns the uniform type identifier of the specified file, if it can be determined.

Deprecated

func localizedDescription(forType: String) -> String?

Returns the localized description for the specified Uniform Type Identifier (UTI).

Deprecated

func preferredFilenameExtension(forType: String) -> String?

Returns the preferred filename extension for the specified Uniform Type Identifier (UTI).

Deprecated

func filenameExtension(String, isValidForType: String) -> Bool

Returns whether the specified filename extension is appropriate for the Uniform Type Identifier (UTI).

Deprecated

func type(String, conformsToType: String) -> Bool

Returns a Boolean indicating that the first Uniform Type Identifier (UTI) conforms to the second UTI.

Deprecated

### Requesting Information

func urlForApplication(toOpen: URL) -> URL?

Returns the URL to the default app to open the specified URL.

func urlForApplication(toOpen: UTType) -> URL?

Returns the URL to the default app to open the specified content type.

func urlForApplication(withBundleIdentifier: String) -> URL?

Returns the URL to the default app with the specified bundle identifier.

func urlsForApplications(toOpen: URL) -> [URL]

Returns an array of URLs to all available applications that can open the URL.

func urlsForApplications(toOpen: UTType) -> [URL]

Returns an array of URLs to all available applications that can open the specified content type.

func urlsForApplications(withBundleIdentifier: String) -> [URL]

Returns an array of URLs to all available applications that can open the specified bundle identifier.

func getFileSystemInfo(forPath: String, isRemovable: UnsafeMutablePointer&lt;ObjCBool>?, isWritable: UnsafeMutablePointer&lt;ObjCBool>?, isUnmountable: UnsafeMutablePointer&lt;ObjCBool>?, description: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, type: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns information about the file system at the specified path.

func isFilePackage(atPath: String) -> Bool

Determines whether the specified path is a file package.

var frontmostApplication: NSRunningApplication?

Returns the frontmost app, which is the app that receives key events.

var runningApplications: [NSRunningApplication]

Returns an array of running apps.

var menuBarOwningApplication: NSRunningApplication?

Returns the app that owns the currently displayed menu bar.

func getInfoForFile(String, application: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, type: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Retrieves information about the specified file.

Deprecated

### Setting Default Application Information

func setDefaultApplication(at: URL, toOpenFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening a specific file.

func setDefaultApplication(at: URL, toOpen: UTType, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type.

func setDefaultApplication(at: URL, toOpenContentTypeOfFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type defined by a file URL.

func setDefaultApplication(at: URL, toOpenURLsWithScheme: String, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific scheme.

### Managing Icons

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func icon(for: UTType) -> NSImage

Returns an image containing the icon for the specified content type.

func setIcon(NSImage?, forFile: String, options: NSWorkspace.IconCreationOptions) -> Bool

Sets the icon for the file or directory at the specified path.

struct IconCreationOptions

Constants that describe options for creating icons.

### Unmounting a Device

func unmountAndEjectDevice(atPath: String) -> Bool

Unmounts and ejects the device at the specified path.

func unmountAndEjectDevice(at: URL) throws

Attempts to eject the volume mounted at the given path.

### Managing the Desktop Image

func desktopImageURL(for: NSScreen) -> URL?

Returns the URL for the desktop image for the given screen.

func setDesktopImageURL(URL, for: NSScreen, options: [NSWorkspace.DesktopImageOptionKey : Any]) throws

Sets the desktop image for the given screen to the image at the specified URL.

func desktopImageOptions(for: NSScreen) -> [NSWorkspace.DesktopImageOptionKey : Any]?

Returns the desktop image options for the given screen.

struct DesktopImageOptionKey

Keys that indicate how to display a new desktop image.

### Performing Finder Spotlight Searches

func showSearchResults(forQueryString: String) -> Bool

Displays a Spotlight search results window in Finder for the specified query string.

### Finder File Labels

var fileLabels: [String]

The array of file labels, returned as strings.

var fileLabelColors: [NSColor]

The array of colors for the file labels.

### Tracking Changes to the File System

func noteFileSystemChanged(String)

Informs the workspace object that the file system changed at the specified path.

### Requesting Additional Time Before Logout

func extendPowerOff(by: Int) -> Int

Requests the system wait for the specified amount of time before turning off the power or logging out the user.

### Supporting Accessibility

var accessibilityDisplayShouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the app avoids conveying information through color alone.

var accessibilityDisplayShouldIncreaseContrast: Bool

A Boolean value that indicates whether the app presents a high-contrast user interface.

var accessibilityDisplayShouldReduceTransparency: Bool

A Boolean value that indicates whether the app avoids using semitransparent backgrounds.

var accessibilityDisplayShouldInvertColors: Bool

A Boolean value that indicates whether the accessibility option to invert colors is in an enabled state.

var accessibilityDisplayShouldReduceMotion: Bool

A Boolean value that indicates whether the accessibility option to reduce motion is in an enabled state.

var isSwitchControlEnabled: Bool

A Boolean value that indicates whether Switch Control is currently running.

var isVoiceOverEnabled: Bool

A Boolean value that indicates whether VoiceOver is currently running.

### Performing Privileged Operations

func requestAuthorization(to: NSWorkspace.AuthorizationType, completionHandler: (NSWorkspace.Authorization?, (any Error)?) -> Void)

Requests authorization to perform a privileged file operation.

class Authorization

The authorization granted to the app by the user.

enum AuthorizationType

The types of privileged file operations that can be authorized by the user.

### Responding to Environment Notifications

class let willLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to launch an app.

class let didLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when a new app starts up.

class let didTerminateApplicationNotification: NSNotification.Name

A notification that the workspace posts when an app finishes executing.

class let sessionDidBecomeActiveNotification: NSNotification.Name

A notification that the workspace posts after a user session switches in.

class let sessionDidResignActiveNotification: NSNotification.Name

A notification that the workspace posts before a user session switches out.

class let didHideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder hides an app.

class let didUnhideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder unhides an app.

class let didActivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to activate an app.

class let didDeactivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder deactivates an app.

class let didRenameVolumeNotification: NSNotification.Name

A notification that the workspace posts when a volume changes its name or mount path.

class let didMountNotification: NSNotification.Name

A notification that the workspace posts when a new device mounts.

class let willUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to unmount a device.

class let didUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder unmounts a device.

class let didChangeFileLabelsNotification: NSNotification.Name

A notification that the workspace posts when the Finder file labels or colors change.

class let activeSpaceDidChangeNotification: NSNotification.Name

A notification that the workspace posts when a Spaces change occurs.

class let didWakeNotification: NSNotification.Name

A notification that the workspace posts when the device wakes from sleep.

class let willPowerOffNotification: NSNotification.Name

A notification that the workspace posts when the user requests a logout or powers off the device.

class let willSleepNotification: NSNotification.Name

A notification that the workspace posts before the device goes to sleep.

class let screensDidSleepNotification: NSNotification.Name

A notification that the workspace posts when the device’s screen goes to sleep.

class let screensDidWakeNotification: NSNotification.Name

A notification that the workspace posts when the device’s screens wake.

class let accessibilityDisplayOptionsDidChangeNotification: NSNotification.Name

A notification that the workspace posts when any of the accessibility display options change.

class let localizedVolumeNameUserInfoKey: String

A string containing the user-visible name of the volume.

class let volumeURLUserInfoKey: String

A URL containing the mount path of the volume.

class let oldLocalizedVolumeNameUserInfoKey: String

A string containing the old user-visible name of the volume

class let oldVolumeURLUserInfoKey: String

A URL containing the old mount path of the volume

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Environment

class OpenConfiguration

The configuration options for opening URLs or launching apps.

struct NSAppKitVersion

Constants for determining which version of AppKit is available.

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

