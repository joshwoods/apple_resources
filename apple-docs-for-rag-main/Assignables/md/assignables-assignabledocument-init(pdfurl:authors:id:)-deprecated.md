

- Assignables
- AssignableDocument
-  init(pdfURL:authors:id:) Deprecated

Initializer

# init(pdfURL:authors:id:)

Initializes a new assessment document that is based on the PDF located at the provided URL. If the file located at the URL provided cannot be accessed, this initializer throws.

iOS 17.4+iPadOS 17.4+visionOSMac Catalyst 17.4+

``` source
init(
    pdfURL: URL,
    authors: [some UserIdentity],
    id: String? = nil
) throws
```

Deprecated

Use init(pdfURL:id:) instead

## Parameters 

`pdfURL`  

A URL to the PDF document that is the basis of this assessment document.

`authors`  

The user identities of contributors to this document. Treated as a set.

`id`  

An optional ID to use for this document. if one is not provided, a random UUID string will be used.

## See Also

### Creating an assignable document

init(pdfURL: URL, id: String?) throws

Initializes a new assessment document that is based on the PDF located at the provided URL. If the file located at the URL provided cannot be accessed, this initializer throws.

