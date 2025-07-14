

- ProximityReader
- MobileNationalIDCardDataRequest
-  MobileNationalIDCardDataRequest.Response 

Structure

# MobileNationalIDCardDataRequest.Response

A type that contains the response information from a successful mobile national ID card data request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Response
```

## Topics

### Structures

struct DocumentElements

A type that contains the document elements from a successful mobile national ID card data request.

### Operators

static func == (MobileNationalIDCardDataRequest.Response, MobileNationalIDCardDataRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let documentElements: MobileNationalIDCardDataRequest.Response.DocumentElements

The document elements from a successful mobile national ID card data request.

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

