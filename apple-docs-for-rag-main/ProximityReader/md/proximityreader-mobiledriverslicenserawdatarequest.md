

- ProximityReader
-  MobileDriversLicenseRawDataRequest 

Structure

# MobileDriversLicenseRawDataRequest

A mobile driver’s license request which retrieves elements from the holder and returns the raw response data for processing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct MobileDriversLicenseRawDataRequest
```

## Topics

### Creating a raw data request

init(retainedElements: [MobileDriversLicenseRawDataRequest.Element], nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element])

Returns a mobile driver’s license raw data request.

var retainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

struct Element

A type representing an element that you can request from a mobile driver’s license.

### Handling the response

struct Response

A type that contains the response information from a successful mobile driver’s license raw data request.

### Operators

static func == (MobileDriversLicenseRawDataRequest, MobileDriversLicenseRawDataRequest) -> Bool

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

struct MobileDriversLicenseDataRequest

A mobile driver’s license request that retrieves elements from the holder and returns the validated document elements.

struct MobileNationalIDCardDisplayRequest

A mobile national ID card request that retrieves elements from the holder and displays the results onscreen for visual inspection.

struct MobileNationalIDCardDataRequest

A mobile national ID card request that retrieves elements from the holder and returns the validated document elements.

struct MobileNationalIDCardRawDataRequest

A mobile national ID card request which retrieves elements from the holder and returns the raw response data for processing.

protocol MobileDocumentRequest

A type that represents a mobile document request.

