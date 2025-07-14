

- WatchKit
- WKRefreshBackgroundTask
-  userInfo 

Instance Property

# userInfo

Custom information associated with the background task.

watchOS 3.0+

``` source
var userInfo: (any NSSecureCoding & NSObjectProtocol)? { get }
```

## Discussion

If there is no data associated with the task, this property is set to `nil`.

