

- UIKit
- UIAccessibility
-  announcementWasSuccessfulUserInfoKey 

Type Property

# announcementWasSuccessfulUserInfoKey

A Boolean value that indicates whether the announcement is successful.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let announcementWasSuccessfulUserInfoKey: String
```

## Discussion

The value of this key is an NSNumber object that the system interprets as a Boolean value.

## See Also

### Notification keys

static let announcementStringValueUserInfoKey: String

The text of the announcement.

static let focusedElementUserInfoKey: String

The element currently in focus by the assistive app.

static let unfocusedElementUserInfoKey: String

The element previously in focus by the assistive app.

static let assistiveTechnologyUserInfoKey: String

The identifier of the assistive app.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

