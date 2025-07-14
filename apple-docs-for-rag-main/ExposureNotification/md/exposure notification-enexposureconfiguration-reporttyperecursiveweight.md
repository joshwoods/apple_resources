

- Exposure Notification
- ENExposureConfiguration
-  reportTypeRecursiveWeight 

Instance Property

# reportTypeRecursiveWeight

The weight assigned to a risk level based on an exposure to someone exposed to someone else.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var reportTypeRecursiveWeight: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

This property is unused.

## See Also

### Configuring Report Types

var reportTypeConfirmedClinicalDiagnosisWeight: Double

The weight assigned to a risk level based on a confirmed clinical diagnosis.

var reportTypeConfirmedTestWeight: Double

The weight assigned to a risk level based on a confirmed test.

var reportTypeSelfReportedWeight: Double

The weight assigned to a risk level based on a self-reported diagnoisis.

var reportTypeNoneMap: ENDiagnosisReportType

The report type to map an unknown diagnosis to.

