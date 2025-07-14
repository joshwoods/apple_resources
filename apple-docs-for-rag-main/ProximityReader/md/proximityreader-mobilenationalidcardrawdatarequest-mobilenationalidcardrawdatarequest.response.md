

- ProximityReader
- MobileNationalIDCardRawDataRequest
-  MobileNationalIDCardRawDataRequest.Response 

Structure

# MobileNationalIDCardRawDataRequest.Response

A type that contains the response information from a successful mobile national ID card raw data request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Response
```

## Topics

### Operators

static func == (MobileNationalIDCardRawDataRequest.Response, MobileNationalIDCardRawDataRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let responseData: Data

The data the mobile national ID card holder returns.

let sessionTranscript: Data

The session transcript of the document request.

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

