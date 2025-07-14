

- WatchKit
- WKURLSessionRefreshBackgroundTask
-  sessionIdentifier 

Instance Property

# sessionIdentifier

The identifier for the triggering background transfer.

watchOS 3.0+

``` source
var sessionIdentifier: String { get }
```

## Discussion

This property holds the background session identifier from the URLSessionConfiguration object used to create the background transfer. Use this identifier to create a configuration and session object to connect to the background session task.

