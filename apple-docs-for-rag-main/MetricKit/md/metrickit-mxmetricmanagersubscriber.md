

- MetricKit
-  MXMetricManagerSubscriber 

Protocol

# MXMetricManagerSubscriber

A protocol defining a method for receiving a daily metrics report.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
protocol MXMetricManagerSubscriber : NSObjectProtocol
```

## Topics

### Receiving reports

func didReceive([MXMetricPayload])

Delivers new metrics reports to the object registered with the metrics manager.

func didReceive([MXDiagnosticPayload])

Delivers new diagnostic reports to the object registered with the metrics manager.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

class MXMetricManager

The shared object that registers you to receive metrics, creates logs for custom metrics, and gives access to past reports.

class MXMetricPayload

An object that encapsulates a daily metrics report.

class MXDiagnosticPayload

An object that encapsulates a diagnostic report.

