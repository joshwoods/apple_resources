

- Foundation
- DistributedNotificationCenter
-  default() 

Type Method

# default()

Returns the default distributed notification center, representing the local notification center for the computer.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func `default`() -> DistributedNotificationCenter
```

## Return Value

Default distributed notification center for the computer.

## Discussion

This method calls forType(_:) with an argument of `NSLocalNotificationCenterType`.

## See Also

### Related Documentation

Notification Programming Topics

### Getting Distributed Notification Centers

class func forType(DistributedNotificationCenter.CenterType) -> DistributedNotificationCenter

Returns the distributed notification center for a particular notification center type.

