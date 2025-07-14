

- AppKit
- NSDocumentController
-  shared 

Type Property

# shared

Returns the shared `NSDocumentController` instance.

macOS

``` source
@MainActor
class var shared: NSDocumentController { get }
```

## Return Value

The shared `NSDocumentController` instance.

## Discussion

If an `NSDocumentController` instance doesn’t exist yet, it is created.

Initialization reads in the document types from the `CFBundleDocumentTypes` property list (in `Info.plist`), registers the instance for willPowerOffNotifications, and turns on the flag indicating that document user interfaces should be visible. You should always obtain your application’s `NSDocumentController` using this method.

## See Also

### Related Documentation

Document-Based App Programming Guide for Mac

