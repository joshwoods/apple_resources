

- HealthKit
- HKFHIRResource
-  identifier 

Instance Property

# identifier

The value from the FHIR resource’s `id` field.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var identifier: String { get }
```

## Mentioned in 

Accessing Health Records

## Discussion

This identifier is only unique for a particular resource type from a given source. To uniquely identify a FHIR resource, you must compare the identifier and resourceType properties from the HKFHIRResource object and the bundleIdentifier property from the clinical record’s source.

## See Also

### Accessing FHIR Data

var fhirVersion: HKFHIRVersion

The FHIR version used by this resource.

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

