

- DeviceActivity
- DeviceActivityFilter
- DeviceActivityFilter.SegmentInterval
-  DeviceActivityFilter.SegmentInterval.hourly(during:) 

Case

# DeviceActivityFilter.SegmentInterval.hourly(during:)

Indicates that the system aggregates data into hourly segments within the specified interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case hourly(during: DateInterval = DateInterval(
                start: Calendar.current.startOfDay(for: .now),
                end: .now
            ))
```

## Discussion

If you do not provide an interval, then the system aggregates device activity into hour-long segments for the current day. The system disregards any date components in the interval that are smaller than `.hour` and instead uses the start of the hour specified by `interval.start` and the end of the hour specified by `interval.end`.

