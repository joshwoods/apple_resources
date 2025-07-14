

- Foundation
- NSUserNotification
-  identifier Deprecated

Instance Property

# identifier

A string that uniquely identifies a notification.

macOS 10.9–11.0Deprecated

``` source
var identifier: String? { get set }
```

## Discussion

The identifier is unique to a notification. A notification delivered with the same identifier as an existing notification replaces the existing notification rather than causing the display of a new notification.

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

var response: NSAttributedString?

The response with which the user responded to a notification.

Deprecated

var responsePlaceholder: String?

Optional placeholder string for inline reply field.

Deprecated

