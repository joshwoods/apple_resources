

- AppKit
-  NSAccessibilityPriorityLevel 

Enumeration

# NSAccessibilityPriorityLevel

A data type for notification priority levels.

macOS 10.9+

``` source
enum NSAccessibilityPriorityLevel
```

## Overview

Use these priority levels as values for the priority key.

## Topics

### Priority Levels

case high

The notification is a high priority.

case medium

The notification is a medium priority.

case low

The notification is a low priority.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

static let announcement: NSAccessibility.NotificationUserInfoKey

The announcement as a localized string.

static let uiElements: NSAccessibility.NotificationUserInfoKey

An array of elements for the notification.

static let priority: NSAccessibility.NotificationUserInfoKey

A priority level that can help an assistive app determine how to handle the corresponding notification.

