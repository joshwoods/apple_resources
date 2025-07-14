

- ProximityReader
-  MobileDriversLicenseDataRequest 

Structure

# MobileDriversLicenseDataRequest

A mobile driver’s license request that retrieves elements from the holder and returns the validated document elements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct MobileDriversLicenseDataRequest
```

## Topics

### Creating a data request

init(retainedElements: [MobileDriversLicenseDataRequest.Element], nonRetainedElements: [MobileDriversLicenseDataRequest.Element])

Returns a mobile driver’s license data request.

var retainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

struct Element

A type that represents an element you can request from a mobile driver’s license.

### Handling the Response

struct Response

A type that contains the response information from a successful mobile driver’s license data request.

### Operators

static func == (MobileDriversLicenseDataRequest, MobileDriversLicenseDataRequest) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

MobileDocumentRequest Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- MobileDocumentRequest
- Sendable

## See Also

### Mobile document requests

struct MobileDriversLicenseDisplayRequest

A mobile driver’s license request that retrieves elements from the holder and displays the results onscreen for visual inspection.

struct MobileDriversLicenseRawDataRequest

A mobile driver’s license request which retrieves elements from the holder and returns the raw response data for processing.

struct MobileNationalIDCardDisplayRequest

A mobile national ID card request that retrieves elements from the holder and displays the results onscreen for visual inspection.

struct MobileNationalIDCardDataRequest

A mobile national ID card request that retrieves elements from the holder and returns the validated document elements.

struct MobileNationalIDCardRawDataRequest

A mobile national ID card request which retrieves elements from the holder and returns the raw response data for processing.

protocol MobileDocumentRequest

A type that represents a mobile document request.

