

- Exposure Notification
- ENExposureConfiguration
-  reportTypeSelfReportedWeight 

Instance Property

# reportTypeSelfReportedWeight

The weight assigned to a risk level based on a self-reported diagnoisis.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var reportTypeSelfReportedWeight: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## See Also

### Configuring Report Types

var reportTypeConfirmedClinicalDiagnosisWeight: Double

The weight assigned to a risk level based on a confirmed clinical diagnosis.

var reportTypeConfirmedTestWeight: Double

The weight assigned to a risk level based on a confirmed test.

var reportTypeRecursiveWeight: Double

The weight assigned to a risk level based on an exposure to someone exposed to someone else.

var reportTypeNoneMap: ENDiagnosisReportType

The report type to map an unknown diagnosis to.

