

- Foundation
-  NSNotificationPostToAllSessions 

Global Variable

# NSNotificationPostToAllSessions

When set, the notification is posted to all sessions. When not set, the notification is sent only to applications within the same login session as the posting task.

Mac Catalyst 13.0+macOS 10.0+

``` source
let NSNotificationPostToAllSessions: DistributedNotificationCenter.Options
```

## See Also

### Constants

let NSNotificationDeliverImmediately: DistributedNotificationCenter.Options

When set, the notification is delivered immediately to all observers, regardless of their suspension behavior or suspension state. When not set, allows the normal suspension behavior of notification observers to take place.

