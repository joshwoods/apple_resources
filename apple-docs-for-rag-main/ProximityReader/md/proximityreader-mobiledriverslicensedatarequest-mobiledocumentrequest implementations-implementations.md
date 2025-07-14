

- ProximityReader
- MobileDriversLicenseDataRequest
-  MobileDocumentRequest Implementations 

API Collection

# MobileDocumentRequest Implementations

## Topics

### Structures

struct Response

A type that contains the response information from a successful mobile driver’s license data request.

### Type Methods

static func driversLicenseData(retaining: [MobileDriversLicenseDataRequest.Element], notRetaining: [MobileDriversLicenseDataRequest.Element]) -> Self

A request which retrieves elements from the holder and returns the validated document elements.

