

- DeviceActivity
- DeviceActivityEvent
-  threshold 

Instance Property

# threshold

The amount of time to monitor the provided applications, categories, and web domains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var threshold: DateComponents { get }
```

## Discussion

Once the activity exceeds the threshold, the system invokes the eventDidReachThreshold(_:activity:) method of the application extension’s principal class.

## See Also

### Including Objects in an Event

var applications: Set&lt;ApplicationToken>

The applications that the event includes.

var categories: Set&lt;ActivityCategoryToken>

The categories that the event includes.

var webDomains: Set&lt;WebDomainToken>

The web domains that the event includes.

