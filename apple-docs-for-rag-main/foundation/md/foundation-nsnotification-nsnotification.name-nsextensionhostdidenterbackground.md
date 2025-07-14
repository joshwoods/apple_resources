

- Foundation
- NSNotification
- NSNotification.Name
-  NSExtensionHostDidEnterBackground 

Type Property

# NSExtensionHostDidEnterBackground

Posted when the extension’s host app begins running in the background.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSExtensionHostDidEnterBackground: NSNotification.Name
```

## Discussion

Extensions can use this notification to stop tasks and prepare the extension to be suspended. The `object` parameter contains the `NSExtensionContext` object. This notification does not contain a `userInfo` dictionary.

Extensions receive only a short amount of time to perform any background work. If you need more time to complete critical tasks, use the methods of the ProcessInfo class to request that time.

## See Also

### Notifications

static let NSExtensionHostDidBecomeActive: NSNotification.Name

Posted when the extension’s host app moves from the inactive to the active state.

static let NSExtensionHostWillResignActive: NSNotification.Name

Posted when the extension’s host app moves from the active to the inactive state.

static let NSExtensionHostWillEnterForeground: NSNotification.Name

Posted when the extension’s host app begins running in the foreground.

