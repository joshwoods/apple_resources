

- AppKit
- NSApplicationDelegate
-  applicationOpenUntitledFile(\_:) 

Instance Method

# applicationOpenUntitledFile(\_:)

Returns a Boolean value that indicates if the app opens an untitled file.

macOS

``` source
@MainActor
optional func applicationOpenUntitledFile(_ sender: NSApplication) -> Bool
```

## Parameters 

`sender`  

The application object associated with the delegate.

## Return Value

true if the file was successfully opened or false if it was not.

## Discussion

Sent directly by `theApplication` to the delegate to request that a new, untitled file be opened.

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

func application(NSApplication, openFiles: [String])

Tells the delegate to open the specified files.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

