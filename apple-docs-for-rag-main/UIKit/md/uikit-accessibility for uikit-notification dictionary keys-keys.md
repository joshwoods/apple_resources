

- UIKit
- Accessibility for UIKit
-  Notification dictionary keys 

API Collection

# Notification dictionary keys

Handle notifications with keys in the user info dictionary.

## Topics

### Notification keys

static let announcementStringValueUserInfoKey: String

The text of the announcement.

static let announcementWasSuccessfulUserInfoKey: String

A Boolean value that indicates whether the announcement is successful.

static let focusedElementUserInfoKey: String

The element currently in focus by the assistive app.

static let unfocusedElementUserInfoKey: String

The element previously in focus by the assistive app.

static let assistiveTechnologyUserInfoKey: String

The identifier of the assistive app.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

## See Also

### Notifications

Notification names

The names of notifications that the accessibility system generates.

static func post(notification: UIAccessibility.Notification, argument: Any?)

Posts a notification to assistive apps.

