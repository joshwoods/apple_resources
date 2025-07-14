

- HealthKit
- HKFHIRResource
-  resourceType 

Instance Property

# resourceType

The value from the FHIR resource’s `resourceType` field.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var resourceType: HKFHIRResourceType { get }
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

struct HKFHIRResourceType

The FHIR resource types supported in HealthKit.

var sourceURL: URL?

The full URL for the source of the FHIR resource.

var data: Data

The JSON representation of the FHIR resource.

