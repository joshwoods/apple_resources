

- Foundation
- NSUserNotification
-  response Deprecated

Instance Property

# response

The response with which the user responded to a notification.

macOS 10.9–11.0Deprecated

``` source
@NSCopying
var response: NSAttributedString? { get }
```

## Discussion

When the user responds to a notification, the NSUserNotificationCenterDelegate method userNotificationCenter(_:didActivate:) is called with the notification, the activationType property set to NSUserNotification.ActivationType.replied, and this property is set with the user’s response.

## See Also

### Display Information

var title: String?

Specifies the title of the notification.

Deprecated

var subtitle: String?

Specifies the subtitle of the notification.

Deprecated

var informativeText: String?

The body text of the notification.

Deprecated

var contentImage: NSImage?

Image shown in the content of the notification.

Deprecated

var identifier: String?

A string that uniquely identifies a notification.

Deprecated

var responsePlaceholder: String?

Optional placeholder string for inline reply field.

Deprecated

