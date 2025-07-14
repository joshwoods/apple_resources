

- HealthKit
- HKFHIRResource
-  sourceURL 

Instance Property

# sourceURL

The full URL for the source of the FHIR resource.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var sourceURL: URL? { get }
```

## Mentioned in 

Accessing Health Records

## See Also

### Accessing FHIR Data

var identifier: String

The value from the FHIR resource’s `id` field.

var fhirVersion: HKFHIRVersion

The FHIR version used by this resource.

class HKFHIRVersion

The FHIR version.

var resourceType: HKFHIRResourceType

The value from the FHIR resource’s `resourceType` field.

struct HKFHIRResourceType

The FHIR resource types supported in HealthKit.

var data: Data

The JSON representation of the FHIR resource.

