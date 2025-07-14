

- HealthKit
- HKStatisticsCollectionQuery
-  intervalComponents 

Instance Property

# intervalComponents

The date components that define the time interval for each statistics object in the collection.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var intervalComponents: DateComponents { get }
```

## Discussion

This property defines the length of the time intervals for your collection. The following code sample shows a number of common time intervals.

- Swift
- Objective-C

```
let fiveMinutes = NSDateComponents()
fiveMinutes.minute = 5

let hour = NSDateComponents()
hour.hour = 1

let day = NSDateComponents()
day.day = 1

let week = NSDateComponents()
week.day = 7

let month = NSDateComponents()
month.month = 1

let year = NSDateComponents()
year.year = 1
```

```
NSDateComponents *fiveMinutes = [[NSDateComponents alloc] init];
fiveMinutes.minute = 5;

NSDateComponents *hour = [[NSDateComponents alloc] init];
hour.hour = 1;

NSDateComponents *day = [[NSDateComponents alloc] init];
day.day = 1;

NSDateComponents *week = [[NSDateComponents alloc] init];
week.day = 7;

NSDateComponents *month = [[NSDateComponents alloc] init];
month.month = 1;

NSDateComponents *year = [[NSDateComponents alloc] init];
year.year = 1;
```

## See Also

### Getting Property Data

var anchorDate: Date

The anchor date for the collection’s time intervals.

var options: HKStatisticsOptions

A list of options that define the type of statistical calculations performed and the way in which data from multiple sources are merged.

