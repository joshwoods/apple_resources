

- AppKit
- NSApplicationDelegate
-  applicationProtectedDataDidBecomeAvailable(\_:) 

Instance Method

# applicationProtectedDataDidBecomeAvailable(\_:)

Tells the delegate that protected data is now available.

macOS 12.0+

``` source
@MainActor
optional func applicationProtectedDataDidBecomeAvailable(_ notification: Notification)
```

## See Also

### Restoring Application State

func applicationSupportsSecureRestorableState(NSApplication) -> Bool

Returns a Boolean value that indicates if the app supports secure state restoration.

func applicationProtectedDataWillBecomeUnavailable(Notification)

Tells the delegate that protected data is about to become unavailable.

func application(NSApplication, willEncodeRestorableState: NSCoder)

Tells the delegate that the app is about to encode its restorable state.

func application(NSApplication, didDecodeRestorableState: NSCoder)

Tells the delegate when the app finished decoding its restorable state.

