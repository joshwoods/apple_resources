

- Assignables
- AssignableDocument
-  init(pdfURL:id:) 

Initializer

# init(pdfURL:id:)

Initializes a new assessment document that is based on the PDF located at the provided URL. If the file located at the URL provided cannot be accessed, this initializer throws.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(
    pdfURL: URL,
    id: String? = nil
) throws
```

## Parameters 

`pdfURL`  

A URL to the PDF document that is the basis of this assessment document.

`id`  

An optional ID to use for this document. if one is not provided, a random UUID string will be used.

## See Also

### Creating an assignable document

init(pdfURL: URL, authors: [some UserIdentity], id: String?) throws

Initializes a new assessment document that is based on the PDF located at the provided URL. If the file located at the URL provided cannot be accessed, this initializer throws.

Deprecated

