

- ProximityReader
- MobileNationalIDCardDataRequest
-  MobileDocumentRequest Implementations 

API Collection

# MobileDocumentRequest Implementations

## Topics

### Structures

struct Response

A type that contains the response information from a successful mobile national ID card data request.

### Type Methods

static func nationalIDCardData(region: Locale.Region, retaining: [MobileNationalIDCardDataRequest.Element], notRetaining: [MobileNationalIDCardDataRequest.Element]) -> Self

A request which retrieves elements from the holder and returns the validated document elements.

