

- AppKit
- NSWorkspace
-  urlsForApplications(toOpen:) 

Instance Method

# urlsForApplications(toOpen:)

Returns an array of URLs to all available applications that can open the URL.

macOS 12.0+

``` source
func urlsForApplications(toOpen url: URL) -> [URL]
```

## Parameters 

`url`  

The URL of the file to open.

## Return Value

An array of URLs to available apps that can open the specified `url`. Returns an empty array if no app can open the URL, or if the file URL doesn’t exist.

## Discussion

The system sorts the resulting array according to each app’s suitability to open the URL. The returned array lists the best match first.

## See Also

### Requesting Information

func urlForApplication(toOpen: URL) -> URL?

Returns the URL to the default app to open the specified URL.

func urlForApplication(toOpen: UTType) -> URL?

Returns the URL to the default app to open the specified content type.

func urlForApplication(withBundleIdentifier: String) -> URL?

Returns the URL to the default app with the specified bundle identifier.

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

