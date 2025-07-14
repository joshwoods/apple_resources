

- Core Foundation
- CFNotificationCenter
-  Notification Posting Options 

API Collection

# Notification Posting Options

Possible options when posting notifications.

## Overview

Use these constants when calling the CFNotificationCenterPostNotificationWithOptions(_:_:_:_:_:) function.

## Topics

### Constants

var kCFNotificationDeliverImmediately: CFOptionFlags

Delivers the notification immediately.

var kCFNotificationPostToAllSessions: CFOptionFlags

Delivers the notification to all sessions.

## See Also

### Constants

enum CFNotificationSuspensionBehavior

Suspension flags that indicate how distributed notifications should be handled when the receiving application is in the background.

