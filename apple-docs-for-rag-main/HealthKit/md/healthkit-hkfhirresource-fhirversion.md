

- HealthKit
- HKFHIRResource
-  fhirVersion 

Instance Property

# fhirVersion

The FHIR version used by this resource.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+

``` source
@NSCopying
var fhirVersion: HKFHIRVersion { get }
```

## See Also

### Accessing FHIR Data

var identifier: String

The value from the FHIR resource’s `id` field.

class HKFHIRVersion

The FHIR version.

var resourceType: HKFHIRResourceType

The value from the FHIR resource’s `resourceType` field.

struct HKFHIRResourceType

The FHIR resource types supported in HealthKit.

var sourceURL: URL?

The full URL for the source of the FHIR resource.

var data: Data

The JSON representation of the FHIR resource.

