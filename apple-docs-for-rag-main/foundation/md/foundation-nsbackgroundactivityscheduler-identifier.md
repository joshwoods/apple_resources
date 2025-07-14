

- Foundation
- NSBackgroundActivityScheduler
-  identifier 

Instance Property

# identifier

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

macOS 10.10+

``` source
var identifier: String { get }
```

## Discussion

This string should remain constant for an activity across launches of your app because the system uses this unique identifier to track the number of times the activity has run and to improve the heuristics for deciding when to run it again in the future. `nil` and zero-length strings are not allowed. See Configure Scheduler Properties.

## See Also

### Related Documentation

init(identifier: String)

Initializes a background activity scheduler object with a specified unique identifier.

### Background Scheduler Attributes

var repeats: Bool

A Boolean value indicating whether the activity should be rescheduled after it completes.

var interval: TimeInterval

An integer providing a suggested interval between scheduling and invoking the activity.

var qualityOfService: QualityOfService

A value of type `NSQualityOfService`, which controls how aggressively the system schedules the activity.

var shouldDefer: Bool

A Boolean value indicating whether your app should stop performing background activity and resume at a more optimal time.

var tolerance: TimeInterval

A value of type TimeInterval, which specifies a range of time during which the background activity may occur.

