

- Exposure Notification
-  ENExposureWindow 

Class

# ENExposureWindow

A set of scan events from observed beacons within a time span.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENExposureWindow
```

## Overview

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

An exposure window contains information about a potential exposure in a 30–minute interval. The system returns an array of exposure windows through the completion handler when the app invokes getExposureWindows(summary:completionHandler:). Exposure windows are only available when an app specified an `ENAPIVersion` of `2` in the app’s `Info.plist` file.

## Topics

### Getting Window Properties

var calibrationConfidence: ENCalibrationConfidence

The transmitting device’s calibration confidence.

var date: Date

The date that the exposure occurred.

var diagnosisReportType: ENDiagnosisReportType

The report type of the observed diagnosis.

var infectiousness: ENInfectiousness

How infectious the user is, based on the number of days since the onset of symptoms.

var scanInstances: [ENScanInstance]

An array of scans corresponding to a beacon associated with an exposure.

var variantOfConcernType: ENVariantOfConcernType

The variant of concern associated with this user.

enum ENVariantOfConcernType

A set of user-definable types that indicate variants of concern.

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

### Exposures

Configuring Exposure Notifications

Define how Exposure Notifications work for a region by assigning server-based key-value pairs.

class ENExposureConfiguration

The object that contains parameters for configuring exposure notification risk scoring behavior.

class ENScanInstance

The aggregation of attenuations of beacons received during a scan.

Exposure Parameter Limits

The limits for the parameters you use in exposure risk calculations.

