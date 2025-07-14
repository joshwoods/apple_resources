

- Foundation
- NSUserNotification
-  title Deprecated

Instance Property

# title

Specifies the title of the notification.

macOS 10.8–11.0Deprecated

``` source
var title: String? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

This value should be localized because it is presented to the user. The string is truncated to a length appropriate for display and the property is modified to reflect the truncation.

## See Also

### Display Information

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

var response: NSAttributedString?

The response with which the user responded to a notification.

Deprecated

var responsePlaceholder: String?

Optional placeholder string for inline reply field.

Deprecated

