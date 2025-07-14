

- Vision
-  VNAnimalIdentifier 

Structure

# VNAnimalIdentifier

An animal identifier string.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct VNAnimalIdentifier
```

## Topics

### Animals

static let cat: VNAnimalIdentifier

An animal identifier for cats.

static let dog: VNAnimalIdentifier

An animal identifier for dogs.

### Initializers

init(rawValue: String)

Creates an identifier with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying Animals

func supportedIdentifiers() throws -> [VNAnimalIdentifier]

Returns the identifiers of the animals that the request detects.

class func knownAnimalIdentifiers(forRevision: Int) throws -> [VNAnimalIdentifier]

Returns a list of animal identifiers the recognition algorithm supports for the specified revision.

Deprecated

