

- AppKit
- NSApplicationDelegate
-  application(\_:openTempFile:) 

Instance Method

# application(\_:openTempFile:)

Returns a Boolean value that indicates if the app opens the specified temporary file.

macOS

``` source
@MainActor
optional func application(
    _ sender: NSApplication,
    openTempFile filename: String
) -> Bool
```

## Parameters 

`sender`  

The application object associated with the delegate.

`filename`  

The name of the temporary file to open.

## Return Value

true if the file was successfully opened or false if it was not.

## Discussion

Sent directly by `theApplication` to the delegate. The method should attempt to open the file `filename`, returning true if the file is successfully opened, and false otherwise.

By design, a file opened through this method is assumed to be temporary—it’s the application’s responsibility to remove the file at the appropriate time.

## See Also

### Opening Files

func application(NSApplication, open: [URL])

Tells the delegate to open the resource at the specified URL.

func application(NSApplication, openFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file.

func application(Any, openFileWithoutUI: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

func application(NSApplication, openFiles: [String])

Tells the delegate to open the specified files.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

