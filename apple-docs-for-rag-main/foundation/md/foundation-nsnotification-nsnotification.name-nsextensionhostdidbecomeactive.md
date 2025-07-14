

- Foundation
- NSNotification
- NSNotification.Name
-  NSExtensionHostDidBecomeActive 

Type Property

# NSExtensionHostDidBecomeActive

Posted when the extension’s host app moves from the inactive to the active state.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSExtensionHostDidBecomeActive: NSNotification.Name
```

## Discussion

Extensions can use this notification to adjust their activity when they become active. The `object` parameter contains the `NSExtensionContext` object. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

static let NSExtensionHostWillResignActive: NSNotification.Name

Posted when the extension’s host app moves from the active to the inactive state.

static let NSExtensionHostDidEnterBackground: NSNotification.Name

Posted when the extension’s host app begins running in the background.

static let NSExtensionHostWillEnterForeground: NSNotification.Name

Posted when the extension’s host app begins running in the foreground.

