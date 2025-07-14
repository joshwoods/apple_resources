

- UIKit
- UIAccessibility
-  UIAccessibility.AssistiveTechnologyIdentifier 

Structure

# UIAccessibility.AssistiveTechnologyIdentifier

Identifiers for assistive apps.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 5.0+

``` source
struct AssistiveTechnologyIdentifier
```

## Overview

Manage pausing and resuming assistive apps with these identifiers.

## Topics

### Identifiers

static let notificationSwitchControl: UIAccessibility.AssistiveTechnologyIdentifier

The Switch Control accessibility feature.

static let notificationVoiceOver: UIAccessibility.AssistiveTechnologyIdentifier

The VoiceOver assistive app.

### Initializer

init(rawValue: String)

Creates an assistive app identifier with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

