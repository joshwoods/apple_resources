

- Foundation
- NSBackgroundActivityScheduler
-  repeats 

Instance Property

# repeats

A Boolean value indicating whether the activity should be rescheduled after it completes.

macOS 10.10+

``` source
var repeats: Bool { get set }
```

## Discussion

The default value for this property is false. See Configure Scheduler Properties.

## See Also

### Background Scheduler Attributes

var identifier: String

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

var interval: TimeInterval

An integer providing a suggested interval between scheduling and invoking the activity.

var qualityOfService: QualityOfService

A value of type `NSQualityOfService`, which controls how aggressively the system schedules the activity.

var shouldDefer: Bool

A Boolean value indicating whether your app should stop performing background activity and resume at a more optimal time.

var tolerance: TimeInterval

A value of type TimeInterval, which specifies a range of time during which the background activity may occur.

