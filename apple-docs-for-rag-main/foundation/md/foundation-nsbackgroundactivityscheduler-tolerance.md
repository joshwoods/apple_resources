

- Foundation
- NSBackgroundActivityScheduler
-  tolerance 

Instance Property

# tolerance

A value of type TimeInterval, which specifies a range of time during which the background activity may occur.

macOS 10.10+

``` source
var tolerance: TimeInterval { get set }
```

## Discussion

A nominal fire date for scheduled background activity is calculated based on a combination of the interval property value and the time the activity began or the last execution date. The tolerance property specifies a grace period—a range of time before and after the nominal fire date, during which the activity may be invoked. As the activity nears the end of its grace period, the system schedules the activity more aggressively. The default tolerance period is half the value of the interval property. See Configure Scheduler Properties.

## See Also

### Related Documentation

typealias TimeInterval

A number of seconds.

### Background Scheduler Attributes

var identifier: String

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

var repeats: Bool

A Boolean value indicating whether the activity should be rescheduled after it completes.

var interval: TimeInterval

An integer providing a suggested interval between scheduling and invoking the activity.

var qualityOfService: QualityOfService

A value of type `NSQualityOfService`, which controls how aggressively the system schedules the activity.

var shouldDefer: Bool

A Boolean value indicating whether your app should stop performing background activity and resume at a more optimal time.

