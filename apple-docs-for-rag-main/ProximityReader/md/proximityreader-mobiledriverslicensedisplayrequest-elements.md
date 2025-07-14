

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  elements 

Instance Property

# elements

The document elements you’re requesting.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var elements: [MobileDriversLicenseDisplayRequest.Element]
```

## Discussion

Note

A request isn’t considered valid if the list of elements is empty, contains duplicates, or contains both age and ageAtLeast(_:). If you call requestDocument(_:) with an invalid request, the framework throws an MobileDocumentReaderError.invalidRequest error.

## See Also

### Creating a display request

init(elements: [MobileDriversLicenseDisplayRequest.Element], options: MobileDriversLicenseDisplayRequest.Options)

Creates a new mobile driver’s license display request.

struct Element

A type that represents an element you can request from a mobile driver’s license.

