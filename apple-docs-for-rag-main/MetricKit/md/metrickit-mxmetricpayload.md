

- MetricKit
-  MXMetricPayload 

Class

# MXMetricPayload

An object that encapsulates a daily metrics report.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXMetricPayload
```

## Topics

### Reading battery metrics

var cellularConditionMetrics: MXCellularConditionMetric?

The cellular condition measurements for the reporting period.

var cpuMetrics: MXCPUMetric?

The CPU metrics for the reporting period.

var displayMetrics: MXDisplayMetric?

The display metrics for the reporting period.

var gpuMetrics: MXGPUMetric?

The GPU metrics for the reporting period.

var locationActivityMetrics: MXLocationActivityMetric?

The location-tracking activity for the reporting period.

var networkTransferMetrics: MXNetworkTransferMetric?

The network-transfer activity for the reporting period.

### Reading performance metrics

var applicationExitMetrics: MXAppExitMetric?

The app foreground and background exit metrics for the reporting period.

var applicationTimeMetrics: MXAppRunTimeMetric?

The app foreground and background time metrics for the reporting period.

var memoryMetrics: MXMemoryMetric?

The memory metrics for the reporting period.

### Reading responsiveness metrics

var applicationLaunchMetrics: MXAppLaunchMetric?

The app launch and resume metrics for the reporting period.

var animationMetrics: MXAnimationMetric?

The metrics for the responsiveness of app animations for the reporting period.

var applicationResponsivenessMetrics: MXAppResponsivenessMetric?

The metrics indicating an app’s responsiveness to user interaction for the reporting period.

### Reading disk access metrics

var diskIOMetrics: MXDiskIOMetric?

The storage metrics for the reporting period.

### Reading custom metrics

var signpostMetrics: [MXSignpostMetric]?

An array of the custom metrics for the reporting period.

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the payload in JSON format.

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the results of the payload as a dictionary.

Deprecated

### Reading information about the payload

var timeStampBegin: Date

The starting time of the reporting period.

var timeStampEnd: Date

The ending time of the reporting period.

var includesMultipleApplicationVersions: Bool

A Boolean indicating if the version of the app changed at least once during the reporting period.

var latestApplicationVersion: String

The version of the app on the device at the end of the reporting period.

var metaData: MXMetaData?

A set of system-level information for the device.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Essentials

class MXMetricManager

The shared object that registers you to receive metrics, creates logs for custom metrics, and gives access to past reports.

class MXDiagnosticPayload

An object that encapsulates a diagnostic report.

protocol MXMetricManagerSubscriber

A protocol defining a method for receiving a daily metrics report.

