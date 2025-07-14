

- HealthKit
-  HKFHIRVersion 

Class

# HKFHIRVersion

The FHIR version.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+

``` source
class HKFHIRVersion
```

## Overview

Use an HKFHIRVersion instance to represent the version of the Fast Healthcare Interoperability Resources (FHIR) standard used to create a HKFHIRResource sample.

## Topics

### Creating Version Objects

convenience init(fromVersionString: String) throws

Creates an FHIR version object from a string representation of the version.

class func primaryDSTU2() -> Self

Returns the primary Second Draft Standard for Trial Use (DSTU2) version.

class func primaryR4() -> Self

Returns the primary Release 4 (R4) version.

### Accessing Version Data

var majorVersion: Int

The standard’s major version number.

var minorVersion: Int

The standard’s minor version number.

var patchVersion: Int

The standard’s patch version number.

var stringRepresentation: String

A string representation of the version.

### Accessing the Release

var fhirRelease: HKFHIRRelease

An official release of the FHIR specification.

struct HKFHIRRelease

Official releases of the FHIR specification.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Accessing FHIR Data

var identifier: String

The value from the FHIR resource’s `id` field.

var fhirVersion: HKFHIRVersion

The FHIR version used by this resource.

var resourceType: HKFHIRResourceType

The value from the FHIR resource’s `resourceType` field.

struct HKFHIRResourceType

The FHIR resource types supported in HealthKit.

var sourceURL: URL?

The full URL for the source of the FHIR resource.

var data: Data

The JSON representation of the FHIR resource.

