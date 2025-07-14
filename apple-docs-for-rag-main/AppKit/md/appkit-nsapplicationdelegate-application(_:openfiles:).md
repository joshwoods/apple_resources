

- AppKit
- NSApplicationDelegate
-  application(\_:openFiles:) 

Instance Method

# application(\_:openFiles:)

Tells the delegate to open the specified files.

macOS

``` source
@MainActor
optional func application(
    _ sender: NSApplication,
    openFiles filenames: [String]
)
```

## Parameters 

`sender`  

The application object associated with the delegate.

`filenames`  

An array of `NSString` objects containing the names of the files to open..

## Discussion

Identical to application(_:openFile:) except that the receiver opens multiple files corresponding to the file names in the `filenames` array. Delegates should invoke the reply(toOpenOrPrint:) method upon success or failure, or when the user cancels the operation.

## See Also

### Opening Files

func application(NSApplication, open: [URL])

Tells the delegate to open the resource at the specified URL.

func application(NSApplication, openFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file.

func application(Any, openFileWithoutUI: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

func application(NSApplication, openTempFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified temporary file.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

