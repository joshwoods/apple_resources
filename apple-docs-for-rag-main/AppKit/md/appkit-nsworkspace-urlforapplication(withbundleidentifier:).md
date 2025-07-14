

- AppKit
- NSWorkspace
-  urlForApplication(withBundleIdentifier:) 

Instance Method

# urlForApplication(withBundleIdentifier:)

Returns the URL to the default app with the specified bundle identifier.

macOS 10.6+

``` source
func urlForApplication(withBundleIdentifier bundleIdentifier: String) -> URL?
```

## Parameters 

`bundleIdentifier`  

The bundle identifier for the app.

## Return Value

The URL of the app, or `nil` if no app has the bundle identifier.

## Discussion

This method uses various heuristics in case multiple apps have the same bundle ID.

You can safely call this method from any thread of your app.

## See Also

### Requesting Information

func urlForApplication(toOpen: URL) -> URL?

Returns the URL to the default app to open the specified URL.

func urlForApplication(toOpen: UTType) -> URL?

Returns the URL to the default app to open the specified content type.

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

