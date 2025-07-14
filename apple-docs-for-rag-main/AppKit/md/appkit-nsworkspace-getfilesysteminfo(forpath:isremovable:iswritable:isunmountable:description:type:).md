

- AppKit
- NSWorkspace
-  getFileSystemInfo(forPath:isRemovable:isWritable:isUnmountable:description:type:) 

Instance Method

# getFileSystemInfo(forPath:isRemovable:isWritable:isUnmountable:description:type:)

Returns information about the file system at the specified path.

macOS

``` source
func getFileSystemInfo(
    forPath fullPath: String,
    isRemovable removableFlag: UnsafeMutablePointer?,
    isWritable writableFlag: UnsafeMutablePointer?,
    isUnmountable unmountableFlag: UnsafeMutablePointer?,
    description: AutoreleasingUnsafeMutablePointer?,
    type fileSystemType: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`fullPath`  

The path to the file system mount point.

`removableFlag`  

On input, a Boolean variable; on return, this variable contains true if the file system is on removable media.

`writableFlag`  

On input, a Boolean variable; on return, this variable contains true if the file system writable.

`unmountableFlag`  

On input, a Boolean variable; on return, this variable contains true if the file system is unmountable.

`description`  

On input, a pointer to a string object variable; on return, if the method was successful, this variable contains a string object that describes the file system. You should not rely on this description for program logic but can use it in message strings. Values can include “hard,” “nfs,” and “foreign.”

`fileSystemType`  

On input, a pointer to a string object variable; on return, if the method was successful, this variable contains the file system type. Values can include “HFS,” “UFS,” or other values.

## Return Value

true if the information was returned; otherwise, false.

## Discussion

You can safely call this method from any thread of your app.

## See Also

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

