

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  MobileDocumentRequest Implementations 

API Collection

# MobileDocumentRequest Implementations

## Topics

### Structures

struct Response

A type that contains the response information from a successful mobile driver’s license raw data request.

### Type Methods

static func driversLicenseRawData(retaining: [MobileDriversLicenseRawDataRequest.Element], notRetaining: [MobileDriversLicenseRawDataRequest.Element]) -> Self

A request which retrieves mobile driver’s license elements from the holder and returns the raw response data for processing.

