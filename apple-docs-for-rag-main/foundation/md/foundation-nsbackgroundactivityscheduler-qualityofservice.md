

- Foundation
- NSBackgroundActivityScheduler
-  qualityOfService 

Instance Property

# qualityOfService

A value of type `NSQualityOfService`, which controls how aggressively the system schedules the activity.

macOS 10.10+

``` source
var qualityOfService: QualityOfService { get set }
```

## Discussion

Options include:

- NSQualityOfServiceUserInteractive

- NSQualityOfServiceUserInitiated

- NSQualityOfServiceUtility

- NSQualityOfServiceBackground

The default value is `NSQualityOfServiceBackground`. If you upgrade the quality of service above this level, the system schedules the activity more aggressively. The default value is the recommended value for most activities. See Configure Scheduler Properties. For information about quality of service, see Prioritize Work at the Task Level in Energy Efficiency Guide for Mac Apps.

## See Also

### Background Scheduler Attributes

var identifier: String

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

var repeats: Bool

A Boolean value indicating whether the activity should be rescheduled after it completes.

var interval: TimeInterval

An integer providing a suggested interval between scheduling and invoking the activity.

var shouldDefer: Bool

A Boolean value indicating whether your app should stop performing background activity and resume at a more optimal time.

var tolerance: TimeInterval

A value of type TimeInterval, which specifies a range of time during which the background activity may occur.

