

- Exposure Notification
-  ENVariantOfConcernType 

Enumeration

# ENVariantOfConcernType

A set of user-definable types that indicate variants of concern.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+

``` source
enum ENVariantOfConcernType
```

## Overview

A Public Health Authority (PHA) defines the meaning of the types that indicate variants of concern. For example, a PHA could define the meaning of ENVariantOfConcernType.type1 as “Vaccine is effective”, and ENVariantOfConcernType.type2 as “Highly transmissive.” The PHA could assign the definition of “High severity” to ENVariantOfConcernType.type3, and “Vaccine breakthrough” to ENVariantOfConcernType.type4.

## Topics

### User-Defined Types

case type1

The first user-definable type for a variant of concern.

case type2

The second user-definable type for a variant of concern.

case type3

The third user-definable type for a variant of concern.

case type4

The fourth user-definable type for a variant of concern.

case typeUnknown

The unknown type for a variant of concern.

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

