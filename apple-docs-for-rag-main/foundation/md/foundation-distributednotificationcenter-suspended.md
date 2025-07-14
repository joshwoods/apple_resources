

- Foundation
- DistributedNotificationCenter
-  suspended 

Instance Property

# suspended

Suspends or resumes notification delivery.

Mac Catalyst 13.0+macOS 10.0+

``` source
var suspended: Bool { get set }
```

## Parameters 

`suspended`  

true suspends notification delivery, false resumes it.

## Discussion

See DistributedNotificationCenter.SuspensionBehavior for details on how the receiver delivers notifications to their observers when normal notification delivery is suspended.

The NSApplication class automatically suspends distributed notification delivery when the application is not active. Applications based on the Application Kit framework should let AppKit manage the suspension of notification delivery. Foundation-only programs may have occasional need to use this method.

## See Also

### Related Documentation

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?, suspensionBehavior: DistributedNotificationCenter.SuspensionBehavior)

Adds an entry to the receiver’s dispatch table with a specific observer and suspended-notifications behavior, and optional notification name and sender.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

