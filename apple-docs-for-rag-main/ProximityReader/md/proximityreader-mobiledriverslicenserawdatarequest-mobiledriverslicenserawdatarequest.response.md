

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  MobileDriversLicenseRawDataRequest.Response 

Structure

# MobileDriversLicenseRawDataRequest.Response

A type that contains the response information from a successful mobile driver’s license raw data request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Response
```

## Topics

### Operators

static func == (MobileDriversLicenseRawDataRequest.Response, MobileDriversLicenseRawDataRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let responseData: Data

The data the mobile driver’s license holder returns.

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

