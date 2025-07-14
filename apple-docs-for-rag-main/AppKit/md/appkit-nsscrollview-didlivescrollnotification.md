

- AppKit
- NSScrollView
-  didLiveScrollNotification 

Type Property

# didLiveScrollNotification

Posted on the main thread after changing the clipview bounds origin due to a user-initiated event.

macOS 10.9+

``` source
class let didLiveScrollNotification: NSNotification.Name
```

## Discussion

Some user-initiated scrolls (for example, scrolling using legacy mice) are not bracketed by a “willStart/didEnd” notification pair.

The notification object is the scroll view performing the scroll.

## See Also

### Notifications

class let willStartLiveMagnifyNotification: NSNotification.Name

Posted at the beginning of a magnify gesture.

class let didEndLiveMagnifyNotification: NSNotification.Name

Posted at the end of a magnify gesture.

class let willStartLiveScrollNotification: NSNotification.Name

Posted on the main thread at the beginning of user-initiated live scroll tracking (gesture scroll or scroller tracking, for example, thumb dragging).

class let didEndLiveScrollNotification: NSNotification.Name

Posted on the main thread at the end of live scroll tracking.

