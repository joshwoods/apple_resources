

- AppKit
- NSWorkspace
-  getInfoForFile(\_:application:type:) Deprecated

Instance Method

# getInfoForFile(\_:application:type:)

Retrieves information about the specified file.

macOS 10.0–12.0Deprecated

``` source
func getInfoForFile(
    _ fullPath: String,
    application appName: AutoreleasingUnsafeMutablePointer?,
    type: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

Deprecated

Use -\[NSWorkspace URLForApplicationToOpenURL:\] to get the URL of an application that will open a given item, or -\[NSURL getResourceValue:forKey:error:\] with NSURLContentTypeKey to get the type of the given item.

## Parameters 

`fullPath`  

The full path to the desired file.

`appName`  

The app the system would use to open the file.

`type`  

On input, a pointer to a string object variable; on return, if the method is successful, this variable contains a string object with the filename extension or encoded HFS file type of the file.

## Return Value

true if this method successfully retrieved the information, or false if it couldn’t find the file or the app isn’t associated with the file.

## Discussion

You can safely call this method from any thread of your app.

## See Also

### Related Documentation

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

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

