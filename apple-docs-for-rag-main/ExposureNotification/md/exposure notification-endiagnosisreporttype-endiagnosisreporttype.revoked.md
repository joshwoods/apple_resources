

- Exposure Notification
- ENDiagnosisReportType
-  ENDiagnosisReportType.revoked 

Case

# ENDiagnosisReportType.revoked

The report is a negative test.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
case revoked
```

## Discussion

This case negates a previous self report or clinical diagnosis that may have been in error.

## See Also

### Enumeration Cases

case confirmedClinicalDiagnosis

The report comes from a confirmed clinical diagnosis.

case confirmedTest

The report comes from a confirmed test.

case recursive

The report comes from a person determined positive based on exposure to another person confirmed positive.

case selfReported

The report comes from the user, without health authority involvement.

case unknown

The report is an unknown type or is not available.

