

- XPC
-  XPC_ACTIVITY_INTERVAL 

Global Variable

# XPC_ACTIVITY_INTERVAL

An integer property that indicates the desired time interval of the activity in seconds.

macOS 10.9+

``` source
let XPC_ACTIVITY_INTERVAL: UnsafePointer
```

## Discussion

The activity doesn’t run more than once per time interval. Due to the nature of XPC Activity finding an opportune time to run the activity, any two occurrences may be more or less than XPC_ACTIVITY_INTERVAL seconds apart, but on average are XPC_ACTIVITY_INTERVAL seconds apart. The presence of this key implies the following, unless you override these values:

- XPC_ACTIVITY_REPEATING with a value of `true`

- XPC_ACTIVITY_DELAY with a value of half the interval. The delay enforces a minimum distance between any two occurrences.

- XPC_ACTIVITY_GRACE_PERIOD with a value of half the interval. The grace period is the amount of time that passes after the end of the interval before more aggressive scheduling occurs. The grace period doesn’t increase the size of the interval.

## See Also

### Time Intervals

let XPC_ACTIVITY_INTERVAL_1_MIN: Int64

A constant that represents a 1-minute time interval.

let XPC_ACTIVITY_INTERVAL_5_MIN: Int64

A constant that represents a 5-minute time interval.

let XPC_ACTIVITY_INTERVAL_15_MIN: Int64

A constant that represents a 15-minute time interval.

let XPC_ACTIVITY_INTERVAL_30_MIN: Int64

A constant that represents a 30-minute time interval.

let XPC_ACTIVITY_INTERVAL_1_HOUR: Int64

A constant that represents a 1-hour time interval.

let XPC_ACTIVITY_INTERVAL_4_HOURS: Int64

A constant that represents a 4-hour time interval.

let XPC_ACTIVITY_INTERVAL_8_HOURS: Int64

A constant that represents an 8-hour time interval.

let XPC_ACTIVITY_INTERVAL_1_DAY: Int64

A constant that represents a one-day time interval.

let XPC_ACTIVITY_INTERVAL_7_DAYS: Int64

A constant that represents a seven-day time interval.

