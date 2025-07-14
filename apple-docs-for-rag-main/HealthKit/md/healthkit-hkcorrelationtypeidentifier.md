

- HealthKit
-  HKCorrelationTypeIdentifier 

Structure

# HKCorrelationTypeIdentifier

The identifiers that create correlation type objects.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKCorrelationTypeIdentifier
```

## Overview

To create an HKCorrelationType instance, pass an HKCorrelationTypeIdentifier value to the correlationType(forIdentifier:) method.

## Topics

### Correlation Types

static let bloodPressure: HKCorrelationTypeIdentifier

A correlation sample that combines a systolic sample and a diastolic sample into a single blood pressure reading.

static let food: HKCorrelationTypeIdentifier

Food correlation types combine any number of nutritional samples into a single food object.

### Initializers

init(rawValue: String)

Returns a newly initialized correlation type identifier using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating correlation types

class func correlationType(forIdentifier: HKCorrelationTypeIdentifier) -> HKCorrelationType?

Returns the shared correlation type for the provided identifier.

