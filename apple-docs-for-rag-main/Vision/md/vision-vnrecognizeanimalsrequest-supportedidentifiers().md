

- Vision
- VNRecognizeAnimalsRequest
-  supportedIdentifiers() 

Instance Method

# supportedIdentifiers()

Returns the identifiers of the animals that the request detects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func supportedIdentifiers() throws -> [VNAnimalIdentifier]
```

## Return Value

The animal identifiers.

## See Also

### Identifying Animals

struct VNAnimalIdentifier

An animal identifier string.

class func knownAnimalIdentifiers(forRevision: Int) throws -> [VNAnimalIdentifier]

Returns a list of animal identifiers the recognition algorithm supports for the specified revision.

Deprecated

