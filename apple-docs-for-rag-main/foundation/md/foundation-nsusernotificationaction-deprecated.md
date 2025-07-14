

- Foundation
-  NSUserNotificationAction Deprecated

Class

# NSUserNotificationAction

An action that the user can take in response to receiving a notification.

macOS 10.10–11.0Deprecated

``` source
class NSUserNotificationAction
```

Deprecated

Use the User Notifications framework instead.

## Overview

User notifications can specify one or more actions to show to the user by using the additionalActivationAction or additionalActions properties. NSUserNotificationAction objects contain the localized title shown to the user and an identifier used to differentiate between presented actions.

## Topics

### Creating User Notification Actions

convenience init(identifier: String?, title: String?)

Creates a user notification action with a specified identifier and title.

### Getting the Identifier and Title

var identifier: String?

The identifier for the user notification action.

var title: String?

The localized title shown to the user.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### User Notifications

class NSUserNotification

A notification that can be scheduled for display in the notification center.

Deprecated

class NSUserNotificationCenter

An object that delivers notifications from apps to the user.

Deprecated

protocol NSUserNotificationCenterDelegate

An interface that enables customizing the behavior of the default notification center.

