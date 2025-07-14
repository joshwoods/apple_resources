

- AppKit
- NSApplicationDelegate
-  applicationSupportsSecureRestorableState(\_:) 

Instance Method

# applicationSupportsSecureRestorableState(\_:)

Returns a Boolean value that indicates if the app supports secure state restoration.

macOS 12.0+

``` source
@MainActor
optional func applicationSupportsSecureRestorableState(_ app: NSApplication) -> Bool
```

## Parameters 

`app`  

The app object associated with the delegate.

## Return Value

`true` when the app supports secure state restoration; otherwise, `false`.

## See Also

### Restoring Application State

func applicationProtectedDataDidBecomeAvailable(Notification)

Tells the delegate that protected data is now available.

func applicationProtectedDataWillBecomeUnavailable(Notification)

Tells the delegate that protected data is about to become unavailable.

func application(NSApplication, willEncodeRestorableState: NSCoder)

Tells the delegate that the app is about to encode its restorable state.

func application(NSApplication, didDecodeRestorableState: NSCoder)

Tells the delegate when the app finished decoding its restorable state.

