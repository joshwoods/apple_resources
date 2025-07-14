

- ProximityReader
- MobileNationalIDCardDisplayRequest
-  elements 

Instance Property

# elements

The document elements you’re requesting.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var elements: [MobileNationalIDCardDisplayRequest.Element]
```

## Discussion

Note

A request isn’t considered valid if the list of elements is empty, contains duplicates, or contains both age and ageAtLeast(_:). If you call requestDocument(_:) with an invalid request, the framework throws an MobileDocumentReaderError.invalidRequest error.

## See Also

### Configuring the request details

var region: Locale.Region

The region of the document you’re requesting.

struct Element

A type that represents an element you can request from a mobile national ID card.

var options: MobileNationalIDCardDisplayRequest.Options

An object that customizes how to perform a display request.

struct Options

An object that customizes how to perform a display request.

