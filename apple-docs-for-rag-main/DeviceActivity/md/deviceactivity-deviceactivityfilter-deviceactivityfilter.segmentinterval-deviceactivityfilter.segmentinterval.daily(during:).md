

- DeviceActivity
- DeviceActivityFilter
- DeviceActivityFilter.SegmentInterval
-  DeviceActivityFilter.SegmentInterval.daily(during:) 

Case

# DeviceActivityFilter.SegmentInterval.daily(during:)

Indicates that the system aggregates data into daily segments within the specified interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case daily(during: DateInterval)
```

## Discussion

The system disregards any date components in the interval that are smaller than `.day` and instead uses the start of the day specified by `interval.start` and the end of the day specified by `interval.end`.

