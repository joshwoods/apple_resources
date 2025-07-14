

- PDFKit
- PDFDocument
-  init(url:) 

Initializer

# init(url:)

Initializes a `PDFDocument` object with the contents at the specified URL (if the URL is invalid, this method returns `NULL`).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
init?(url: URL)
```

## Return Value

A `PDFDocument` instance initialized with the data at the passed-in URL or `NULL` if the object could not be initialized or if the URL is invalid.

## See Also

### Initializing Documents

init?(data: Data)

Initializes a `PDFDocument` object with the passed-in data.

init()

Initializes a `PDFDocument` object.

