

- AppKit
- NSScrollView
-  willStartLiveMagnifyNotification 

Type Property

# willStartLiveMagnifyNotification

Posted at the beginning of a magnify gesture.

macOS 10.8+

``` source
class let willStartLiveMagnifyNotification: NSNotification.Name
```

## Discussion

The notification object is the scroll view performing the magnification.

This notification indicates that the magnification property is being changed due to user action. This may be due to the user performing a pinch gesture or a smart zoom gesture. When animating the magnification value yourself via the object’s animator, this notification is not sent.

## See Also

### Notifications

class let didEndLiveMagnifyNotification: NSNotification.Name

Posted at the end of a magnify gesture.

class let willStartLiveScrollNotification: NSNotification.Name

Posted on the main thread at the beginning of user-initiated live scroll tracking (gesture scroll or scroller tracking, for example, thumb dragging).

class let didLiveScrollNotification: NSNotification.Name

Posted on the main thread after changing the clipview bounds origin due to a user-initiated event.

class let didEndLiveScrollNotification: NSNotification.Name

Posted on the main thread at the end of live scroll tracking.

