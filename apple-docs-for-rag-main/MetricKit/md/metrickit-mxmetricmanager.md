

- MetricKit
-  MXMetricManager 

Class

# MXMetricManager

The shared object that registers you to receive metrics, creates logs for custom metrics, and gives access to past reports.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
class MXMetricManager
```

## Overview

The `MXMetricManager` shared object manages your subscription for receiving on-device daily metrics.

MetricKit starts accumulating reports for your app after calling shared for the first time. To receive the reports, call add(_:) with an object that adopts the MXMetricManagerSubscriber protocol. The system then delivers metric reports at most once per day, and diagnostic reports immediately in iOS 15 and later and macOS 12 and later. The reports contain the metrics from the past 24 hours and any previously undelivered daily reports. To pause receiving reports, call remove(_:).

The calls to add a subscriber and for receiving reports are safe to use in performance-sensitive code, such as app launch.

The snippet below shows a simple class for using MetricKit.

```
```

## Topics

### Getting the shared metrics manager

class var shared: MXMetricManager

An object that returns the shared metrics manager instance.

### Subscribing to reports

func add(any MXMetricManagerSubscriber)

Registers to receive a daily report of app metrics from the metrics manager.

func remove(any MXMetricManagerSubscriber)

Unsubscribes from daily reports of app metrics.

### Retrieving previous reports

var pastPayloads: [MXMetricPayload]

Returns an array of the daily metrics reports generated since the last allocation of the shared manager instance.

var pastDiagnosticPayloads: [MXDiagnosticPayload]

Returns an array of the diagnostic reports generated since the last allocation of the shared manager instance.

### Creating custom metric logs

class func makeLogHandle(category: String) -> OSLog

Returns a log handle used for writing custom metric events.

### Measuring an extended launch

class func extendLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Starts to measure an extended launch task with the given task identifier.

class func finishExtendedLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Signals the end of an extended launch task.

struct MXLaunchTaskID

The task identifier to track launch measurements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

class MXMetricPayload

An object that encapsulates a daily metrics report.

class MXDiagnosticPayload

An object that encapsulates a diagnostic report.

protocol MXMetricManagerSubscriber

A protocol defining a method for receiving a daily metrics report.

