

- AppKit
- NSApplicationDelegate
-  application(\_:openFile:) 

Instance Method

# application(\_:openFile:)

Returns a Boolean value that indicates if the app opens the specified file.

macOS

``` source
@MainActor
optional func application(
    _ sender: NSApplication,
    openFile filename: String
) -> Bool
```

## Parameters 

`sender`  

The application object associated with the delegate.

`filename`  

The name of the file to open.

## Return Value

true if the file was successfully opened or false if it was not.

## Discussion

Sent directly by `theApplication` to the delegate. The method should open the file `filename`, returning true if the file is successfully opened, and false otherwise. If the user started up the application by double-clicking a file, the delegate receives the application(_:openFile:) message before receiving applicationDidFinishLaunching(_:). (applicationWillFinishLaunching(_:) is sent before application(_:openFile:).)

## See Also

### Opening Files

func application(NSApplication, open: [URL])

Tells the delegate to open the resource at the specified URL.

func application(Any, openFileWithoutUI: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

func application(NSApplication, openTempFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified temporary file.

func application(NSApplication, openFiles: [String])

Tells the delegate to open the specified files.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

