

- HealthKit
-  HKFHIRRelease 

Structure

# HKFHIRRelease

Official releases of the FHIR specification.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKFHIRRelease
```

## Overview

Each release can have multiple versions.

## Topics

### Releases

static let dstu2: HKFHIRRelease

The Second Draft Standard for Trial Use (DSTU2) release.

static let r4: HKFHIRRelease

The Release 4 (R4) release.

static let unknown: HKFHIRRelease

An unknown release.

### Initializers

init(rawValue: String)

Creates a new release from the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the Release

var fhirRelease: HKFHIRRelease

An official release of the FHIR specification.

