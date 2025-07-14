

- DeviceActivity
- DeviceActivityEvent
-  applications 

Instance Property

# applications

The applications that the event includes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var applications: Set { get }
```

## See Also

### Including Objects in an Event

var categories: Set&lt;ActivityCategoryToken>

The categories that the event includes.

var webDomains: Set&lt;WebDomainToken>

The web domains that the event includes.

var threshold: DateComponents

The amount of time to monitor the provided applications, categories, and web domains.

