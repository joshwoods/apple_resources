

- Exposure Notification
-  ENInfectiousness 

Enumeration

# ENInfectiousness

The degree to which a person’s symptoms may indicate transmission risk.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
enum ENInfectiousness
```

## Overview

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

## Topics

### Enumeration Cases

case high

The user is highly infectious.

case none

The user is not infectious.

case standard

The user is mildly infectious.

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

enum ENDiagnosisReportType

The type of a report that describes the origin of a diagnosis.

