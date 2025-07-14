

- ProximityReader
- MobileNationalIDCardRawDataRequest
-  MobileDocumentRequest Implementations 

API Collection

# MobileDocumentRequest Implementations

## Topics

### Structures

struct Response

A type that contains the response information from a successful mobile national ID card raw data request.

### Type Methods

static func nationalIDCardRawData(region: Locale.Region, retaining: [MobileNationalIDCardRawDataRequest.Element], notRetaining: [MobileNationalIDCardRawDataRequest.Element]) -> Self

A request which retrieves mobile national ID card elements from the holder and returns the raw response data for processing.

