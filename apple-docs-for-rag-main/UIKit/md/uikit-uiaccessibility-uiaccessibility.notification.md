

- UIKit
- UIAccessibility
-  UIAccessibility.Notification 

Structure

# UIAccessibility.Notification

An accessibility notification that an app can send.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
struct Notification
```

## Topics

### Notifications

static let announcement: UIAccessibility.Notification

A notification that an app posts when it needs to convey an announcement to the assistive app.

static let layoutChanged: UIAccessibility.Notification

A notification that an app posts when the layout of a screen changes.

static let screenChanged: UIAccessibility.Notification

A notification that an app posts when a new view appears that occupies a major portion of the screen.

static let pageScrolled: UIAccessibility.Notification

A notification that an app posts when a scroll action completes.

static let pauseAssistiveTechnology: UIAccessibility.Notification

A notification that pauses an assistive app’s operations temporarily.

static let resumeAssistiveTechnology: UIAccessibility.Notification

A notification that resumes an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

### Initializer

init(rawValue: UInt32)

Creates an accessibility notification with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling notifications

Notification names

The names of notifications that the accessibility system generates.

Notification dictionary keys

Handle notifications with keys in the user info dictionary.

static func post(notification: UIAccessibility.Notification, argument: Any?)

Posts a notification to assistive apps.

