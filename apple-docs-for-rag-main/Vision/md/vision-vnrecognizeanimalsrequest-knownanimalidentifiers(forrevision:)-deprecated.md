

- Vision
- VNRecognizeAnimalsRequest
-  knownAnimalIdentifiers(forRevision:) Deprecated

Type Method

# knownAnimalIdentifiers(forRevision:)

Returns a list of animal identifiers the recognition algorithm supports for the specified revision.

iOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func knownAnimalIdentifiers(forRevision requestRevision: Int) throws -> [VNAnimalIdentifier]
```

Deprecated

Use supportedIdentifiers() instead.

## Parameters 

`requestRevision`  

The revision of the animal recognition request.

## Return Value

The animal identifiers.

## See Also

### Identifying Animals

func supportedIdentifiers() throws -> [VNAnimalIdentifier]

Returns the identifiers of the animals that the request detects.

struct VNAnimalIdentifier

An animal identifier string.

