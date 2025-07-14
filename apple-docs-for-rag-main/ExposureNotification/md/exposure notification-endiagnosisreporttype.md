

- Exposure Notification
-  ENDiagnosisReportType 

Enumeration

# ENDiagnosisReportType

The type of a report that describes the origin of a diagnosis.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
enum ENDiagnosisReportType
```

## Overview

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## Topics

### Enumeration Cases

case confirmedClinicalDiagnosis

The report comes from a confirmed clinical diagnosis.

case confirmedTest

The report comes from a confirmed test.

case recursive

The report comes from a person determined positive based on exposure to another person confirmed positive.

case revoked

The report is a negative test.

case selfReported

The report comes from the user, without health authority involvement.

case unknown

The report is an unknown type or is not available.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

Attenuation

The minimum and maximum signal attenuations.

Risk Level

The minimum and maximum risk levels.

Risk Level Value

The minimum and maximum risk level values.

Risk Score

The minimum and maximum risk score.

Risk Weight

The minimum, default, and maximum risk weights.

struct ENActivityFlags

Activities that occur while the app isn’t running.

enum ENCalibrationConfidence

The transmitting device’s calibration confidence.

enum ENInfectiousness

The degree to which a person’s symptoms may indicate transmission risk.

