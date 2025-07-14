

- ProximityReader
- MobileDriversLicenseDataRequest
-  MobileDriversLicenseDataRequest.Response 

Structure

# MobileDriversLicenseDataRequest.Response

A type that contains the response information from a successful mobile driver’s license data request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Response
```

## Topics

### Structures

struct DocumentElements

A type that contains the document elements from a successful mobile driver’s license data request.

### Operators

static func == (MobileDriversLicenseDataRequest.Response, MobileDriversLicenseDataRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let documentElements: MobileDriversLicenseDataRequest.Response.DocumentElements

The document elements from a successful mobile driver’s license data request.

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

