

- ProximityReader
- MobileNationalIDCardDisplayRequest
- MobileNationalIDCardDisplayRequest.Response
-  MobileNationalIDCardDisplayRequest.Response.ValidationOutcome 

Enumeration

# MobileNationalIDCardDisplayRequest.Response.ValidationOutcome

A type that represents how the user validates the mobile document response.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum ValidationOutcome
```

## Topics

### Operators

static func == (MobileNationalIDCardDisplayRequest.Response.ValidationOutcome, MobileNationalIDCardDisplayRequest.Response.ValidationOutcome) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case approved

A message that indicates the user approved the document response.

case dismissed

A message that indicates the user didn’t explicitly approve or reject the document response.

case rejected

A message that indicates the user rejected the document response.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

