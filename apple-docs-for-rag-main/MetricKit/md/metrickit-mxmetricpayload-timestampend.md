

- MetricKit
- MXMetricPayload
-  timeStampEnd 

Instance Property

# timeStampEnd

The ending time of the reporting period.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var timeStampEnd: Date { get }
```

## See Also

### Reading information about the payload

var timeStampBegin: Date

The starting time of the reporting period.

var includesMultipleApplicationVersions: Bool

A Boolean indicating if the version of the app changed at least once during the reporting period.

var latestApplicationVersion: String

The version of the app on the device at the end of the reporting period.

var metaData: MXMetaData?

A set of system-level information for the device.

