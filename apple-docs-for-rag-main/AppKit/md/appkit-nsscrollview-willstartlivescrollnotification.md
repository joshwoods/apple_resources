

- AppKit
- NSScrollView
-  willStartLiveScrollNotification 

Type Property

# willStartLiveScrollNotification

Posted on the main thread at the beginning of user-initiated live scroll tracking (gesture scroll or scroller tracking, for example, thumb dragging).

macOS 10.9+

``` source
class let willStartLiveScrollNotification: NSNotification.Name
```

## Discussion

The notification object is the scroll view performing the scroll.

## See Also

### Notifications

class let willStartLiveMagnifyNotification: NSNotification.Name

Posted at the beginning of a magnify gesture.

class let didEndLiveMagnifyNotification: NSNotification.Name

Posted at the end of a magnify gesture.

class let didLiveScrollNotification: NSNotification.Name

Posted on the main thread after changing the clipview bounds origin due to a user-initiated event.

class let didEndLiveScrollNotification: NSNotification.Name

Posted on the main thread at the end of live scroll tracking.

