

- ProximityReader
-  MobileDocumentRequest 

Protocol

# MobileDocumentRequest

A type that represents a mobile document request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
protocol MobileDocumentRequest : Hashable, Sendable
```

## Mentioned in 

Adopting the Verifier API in your iPhone app

## Topics

### Mobile driver’s license display request

struct MobileDriversLicenseDisplayRequest

A mobile driver’s license request that retrieves elements from the holder and displays the results onscreen for visual inspection.

static func displayDriversLicense([MobileDriversLicenseDisplayRequest.Element], options: MobileDriversLicenseDisplayRequest.Options) -> Self

A request that displays driver’s license elements onscreen.

### Mobile driver’s license data request

struct MobileDriversLicenseDataRequest

A mobile driver’s license request that retrieves elements from the holder and returns the validated document elements.

static func driversLicenseData(retaining: [MobileDriversLicenseDataRequest.Element], notRetaining: [MobileDriversLicenseDataRequest.Element]) -> Self

A request which retrieves elements from the holder and returns the validated document elements.

### Mobile driver’s license raw data request

struct MobileDriversLicenseRawDataRequest

A mobile driver’s license request which retrieves elements from the holder and returns the raw response data for processing.

static func driversLicenseRawData(retaining: [MobileDriversLicenseRawDataRequest.Element], notRetaining: [MobileDriversLicenseRawDataRequest.Element]) -> Self

A request which retrieves mobile driver’s license elements from the holder and returns the raw response data for processing.

### National ID card display request

struct MobileNationalIDCardDisplayRequest

A mobile national ID card request that retrieves elements from the holder and displays the results onscreen for visual inspection.

static func nationalIDCard(region: Locale.Region, [MobileNationalIDCardDisplayRequest.Element], options: MobileNationalIDCardDisplayRequest.Options) -> Self

A request that displays national ID card elements onscreen.

### National ID card license data request

struct MobileNationalIDCardDataRequest

A mobile national ID card request that retrieves elements from the holder and returns the validated document elements.

static func nationalIDCardData(region: Locale.Region, retaining: [MobileNationalIDCardDataRequest.Element], notRetaining: [MobileNationalIDCardDataRequest.Element]) -> Self

A request which retrieves elements from the holder and returns the validated document elements.

### National ID card license raw data request

struct MobileNationalIDCardRawDataRequest

A mobile national ID card request which retrieves elements from the holder and returns the raw response data for processing.

static func nationalIDCardRawData(region: Locale.Region, retaining: [MobileNationalIDCardRawDataRequest.Element], notRetaining: [MobileNationalIDCardRawDataRequest.Element]) -> Self

A request which retrieves mobile national ID card elements from the holder and returns the raw response data for processing.

### Associated Types

associatedtype Response : Hashable, Sendable

A type that represents the response type of the request.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- MobileDriversLicenseDataRequest
- MobileDriversLicenseDisplayRequest
- MobileDriversLicenseRawDataRequest
- MobileNationalIDCardDataRequest
- MobileNationalIDCardDisplayRequest
- MobileNationalIDCardRawDataRequest

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

struct MobileNationalIDCardRawDataRequest

A mobile national ID card request which retrieves elements from the holder and returns the raw response data for processing.

