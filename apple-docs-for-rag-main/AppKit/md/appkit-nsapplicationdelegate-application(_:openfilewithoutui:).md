

- AppKit
- NSApplicationDelegate
-  application(\_:openFileWithoutUI:) 

Instance Method

# application(\_:openFileWithoutUI:)

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

macOS

``` source
@MainActor
optional func application(
    _ sender: Any,
    openFileWithoutUI filename: String
) -> Bool
```

## Parameters 

`sender`  

The object that sent the command.

`filename`  

The name of the file to open.

## Return Value

true if the file was successfully opened or false if it was not.

## Discussion

Sent directly by `sender` to the delegate to request that the file `filename` be opened as a linked file. The method should open the file without bringing up its application’s user interface—that is, work with the file is under programmatic control of `sender`, rather than under keyboard control of the user.

## See Also

### Related Documentation

func application(NSApplication, printFile: String) -> Bool

Returns a Boolean value that indicates if the app prints the specified file in its entirety.

### Opening Files

func application(NSApplication, open: [URL])

Tells the delegate to open the resource at the specified URL.

func application(NSApplication, openFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file.

func application(NSApplication, openTempFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified temporary file.

func application(NSApplication, openFiles: [String])

Tells the delegate to open the specified files.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

