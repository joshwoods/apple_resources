

- DeviceActivity
- DeviceActivityFilter
- DeviceActivityFilter.SegmentInterval
-  DeviceActivityFilter.SegmentInterval.weekly(during:) 

Case

# DeviceActivityFilter.SegmentInterval.weekly(during:)

Indicates that the system aggregates data into weekly segments within the specified interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case weekly(during: DateInterval)
```

## Discussion

The system disregards any date components in the interval that are smaller than `.weekOfYear` and instead uses the start of the week specified by `interval.start` and the end of the week specified by `interval.end`.

