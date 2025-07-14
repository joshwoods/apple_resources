

- Exposure Notification
- ENExposureWindow
-  calibrationConfidence 

Instance Property

# calibrationConfidence

The transmitting device’s calibration confidence.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var calibrationConfidence: ENCalibrationConfidence { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## See Also

### Getting Window Properties

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

