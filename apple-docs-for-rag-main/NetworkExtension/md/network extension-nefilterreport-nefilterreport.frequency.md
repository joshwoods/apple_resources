

- Network Extension
- NEFilterReport
-  NEFilterReport.Frequency 

Enumeration

# NEFilterReport.Frequency

An enumeration that represents the frequency of filter report delivery.

macOS 10.15.4+

``` source
enum Frequency
```

## Topics

### Report frequencies

case none

A frequency value that indicates no report delivery.

case low

A low frequency of reports, about once every five seconds.

case medium

A low frequency of reports, about once every second.

case high

A low frequency of reports, about once every half-second.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting new flow verdict properties

var statisticsReportFrequency: NEFilterReport.Frequency

The frequency at which the data provider receives reports.

