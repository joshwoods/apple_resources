

- ProximityReader
-  MobileNationalIDCardRawDataRequest 

Structure

# MobileNationalIDCardRawDataRequest

A mobile national ID card request which retrieves elements from the holder and returns the raw response data for processing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct MobileNationalIDCardRawDataRequest
```

## Topics

### Creating a raw data request

init(region: Locale.Region, retainedElements: [MobileNationalIDCardRawDataRequest.Element], nonRetainedElements: [MobileNationalIDCardRawDataRequest.Element])

Creates a mobile national ID card raw data request.

### Determining the region availability

static func isSupportedRegion(Locale.Region) -> Bool

Returns a Boolean value that indicates whether you can make a request for the specified region.

### Configuring the request details

var region: Locale.Region

The region of the document you’re requesting.

var retainedElements: [MobileNationalIDCardRawDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileNationalIDCardRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

struct Element

A type representing an element that you can request from a mobile national ID card.

### Handling the response

struct Response

A type that contains the response information from a successful mobile national ID card raw data request.

### Operators

static func == (MobileNationalIDCardRawDataRequest, MobileNationalIDCardRawDataRequest) -> Bool

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

struct MobileDriversLicenseRawDataRequest

A mobile driver’s license request which retrieves elements from the holder and returns the raw response data for processing.

struct MobileNationalIDCardDisplayRequest

A mobile national ID card request that retrieves elements from the holder and displays the results onscreen for visual inspection.

struct MobileNationalIDCardDataRequest

A mobile national ID card request that retrieves elements from the holder and returns the validated document elements.

protocol MobileDocumentRequest

A type that represents a mobile document request.

