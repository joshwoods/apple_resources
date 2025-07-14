

- ProximityReader
-  MobileDriversLicenseDisplayRequest 

Structure

# MobileDriversLicenseDisplayRequest

A mobile driver’s license request that retrieves elements from the holder and displays the results onscreen for visual inspection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct MobileDriversLicenseDisplayRequest
```

## Topics

### Creating a display request

init(elements: [MobileDriversLicenseDisplayRequest.Element], options: MobileDriversLicenseDisplayRequest.Options)

Creates a new mobile driver’s license display request.

var elements: [MobileDriversLicenseDisplayRequest.Element]

The document elements you’re requesting.

struct Element

A type that represents an element you can request from a mobile driver’s license.

### Configuring a display request

var options: MobileDriversLicenseDisplayRequest.Options

An object that customizes how to perform a display request.

struct Options

An object that customizes how to perform a display request.

### Handling the response

struct Response

A type that contains the response information from a successful mobile driver’s license display request.

### Operators

static func == (MobileDriversLicenseDisplayRequest, MobileDriversLicenseDisplayRequest) -> Bool

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

struct MobileDriversLicenseDataRequest

A mobile driver’s license request that retrieves elements from the holder and returns the validated document elements.

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

