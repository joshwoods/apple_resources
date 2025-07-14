

- AppKit
- NSApplicationDelegate
-  application(\_:open:) 

Instance Method

# application(\_:open:)

Tells the delegate to open the resource at the specified URL.

macOS 10.13+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    open urls: [URL]
)
```

## Parameters 

`application`  

Your singleton app object.

`urls`  

An array of URLs to open. The list does not include URLs for which your app has a defined document type.

## Discussion

AppKit calls this method when your app is asked to open one or more URL-based resources. You must declare the URL types that your app supports in your `Info.plist` file using the `CFBundleURLTypes` key. The list can also include URLs for documents for which your app does not have an associated NSDocument class. You configure document types using Xcode, or by adding the `CFBundleDocumentTypes` key to your `Info.plist` file.

If your delegate implements this method, AppKit does not call the application(_:openFile:) or application(_:openFiles:) methods.

## See Also

### Opening Files

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

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

