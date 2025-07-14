

- DeviceActivity
- DeviceActivityEvent
-  includesAllActivity 

Instance Property

# includesAllActivity

A Boolean value that indicates whether the event includes all applications, categories, and web domains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var includesAllActivity: Bool { get }
```

## Discussion

Use `includesAllActivity` to determine the content of the scheduled event. Evaluates to `true` if applications, categories, and webDomains are empty; otherwise `false`.

## See Also

### Creating an Event

init(applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>, threshold: DateComponents)

Creates a new event.

struct Name

The unique name of an event.

