

- Foundation
- NSNotification
- NSNotification.Name
-  NSExtensionHostWillResignActive 

Type Property

# NSExtensionHostWillResignActive

Posted when the extension’s host app moves from the active to the inactive state.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSExtensionHostWillResignActive: NSNotification.Name
```

## Discussion

Extensions can use this notification to adjust their activity when they become inactive. For example, you might use this notification to save any unsaved data to prevent it from being lost. The `object` parameter contains the `NSExtensionContext` object. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

static let NSExtensionHostDidBecomeActive: NSNotification.Name

Posted when the extension’s host app moves from the inactive to the active state.

static let NSExtensionHostDidEnterBackground: NSNotification.Name

Posted when the extension’s host app begins running in the background.

static let NSExtensionHostWillEnterForeground: NSNotification.Name

Posted when the extension’s host app begins running in the foreground.

