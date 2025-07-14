

- AppKit
- NSApplicationDelegate
-  application(\_:willEncodeRestorableState:) 

Instance Method

# application(\_:willEncodeRestorableState:)

Tells the delegate that the app is about to encode its restorable state.

macOS 10.7+

``` source
@MainActor
optional func application(
    _ app: NSApplication,
    willEncodeRestorableState coder: NSCoder
)
```

## Parameters 

`app`  

The application.

`coder`  

The coder extracting the archive.

## See Also

### Restoring Application State

func applicationSupportsSecureRestorableState(NSApplication) -> Bool

Returns a Boolean value that indicates if the app supports secure state restoration.

func applicationProtectedDataDidBecomeAvailable(Notification)

Tells the delegate that protected data is now available.

func applicationProtectedDataWillBecomeUnavailable(Notification)

Tells the delegate that protected data is about to become unavailable.

func application(NSApplication, didDecodeRestorableState: NSCoder)

Tells the delegate when the app finished decoding its restorable state.

