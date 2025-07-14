

- HealthKit
- HKObjectType
-  requiresPerObjectAuthorization() 

Instance Method

# requiresPerObjectAuthorization()

Returns a Boolean that indicates whether the data type requires per-object authorization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func requiresPerObjectAuthorization() -> Bool
```

## Discussion

If this method returns true, you must call requestPerObjectReadAuthorization(for:predicate:completion:) each time you want to query for the data type. The user can then select the individual samples that the app has permission to read. The system always prompts the user for permission, regardless of whether they’ve previously granted permission.

Important

Using the requestAuthorization(toShare:read:) method to request read access to any data types that require per-object authorization fails with an HKError.Code.errorInvalidArgument error.

## See Also

### Related Documentation

class HKPrescriptionType

A type that identifies samples that store a prescription.

let HKVisionPrescriptionTypeIdentifier: String

A type identifier for vision prescription samples.

### Getting property data

var identifier: String

A unique string identifying the HealthKit object type.

