

- Foundation
- NSBackgroundActivityScheduler
-  interval 

Instance Property

# interval

An integer providing a suggested interval between scheduling and invoking the activity.

macOS 10.10+

``` source
var interval: TimeInterval { get set }
```

## Discussion

For repeating activities, the value of this property is also the suggested interval between invocations. See Configure Scheduler Properties.

## See Also

### Background Scheduler Attributes

var identifier: String

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

var repeats: Bool

A Boolean value indicating whether the activity should be rescheduled after it completes.

var qualityOfService: QualityOfService

A value of type `NSQualityOfService`, which controls how aggressively the system schedules the activity.

var shouldDefer: Bool

A Boolean value indicating whether your app should stop performing background activity and resume at a more optimal time.

var tolerance: TimeInterval

A value of type TimeInterval, which specifies a range of time during which the background activity may occur.

