

- AppKit
- NSApplicationDelegate
-  applicationShouldOpenUntitledFile(\_:) 

Instance Method

# applicationShouldOpenUntitledFile(\_:)

Returns a Boolean value that indicates if the app can open an untitled file.

macOS

``` source
@MainActor
optional func applicationShouldOpenUntitledFile(_ sender: NSApplication) -> Bool
```

## Parameters 

`sender`  

The application object associated with the delegate.

## Return Value

true if the application should open a new untitled file or false if it should not.

## Discussion

Use this method to decide whether the application should open a new, untitled file. Note that applicationOpenUntitledFile(_:) is invoked if this method returns true.

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

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

