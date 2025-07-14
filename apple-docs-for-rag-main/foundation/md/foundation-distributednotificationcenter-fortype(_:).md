

- Foundation
- DistributedNotificationCenter
-  forType(\_:) 

Type Method

# forType(\_:)

Returns the distributed notification center for a particular notification center type.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func forType(_ notificationCenterType: DistributedNotificationCenter.CenterType) -> DistributedNotificationCenter
```

## Parameters 

`notificationCenterType`  

Notification center type being inquired about.

## Return Value

Distributed notification center for `notificationCenterType`.

## Discussion

Currently only one type, `NSLocalNotificationCenterType`, is supported.

## See Also

### Getting Distributed Notification Centers

class func `default`() -> DistributedNotificationCenter

Returns the default distributed notification center, representing the local notification center for the computer.

