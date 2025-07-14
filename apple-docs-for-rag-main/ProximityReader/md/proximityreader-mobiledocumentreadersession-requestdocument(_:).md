

- ProximityReader
- MobileDocumentReaderSession
-  requestDocument(\_:) 

Instance Method

# requestDocument(\_:)

Presents a sheet to read a mobile document and returns the relevant response.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
@discardableResult
final func requestDocument(_ request: Request) async throws -> Request.Response where Request : MobileDocumentRequest
```

## Parameters 

`request`  

The mobile document request.

## Return Value

A Response if the request was successful.

## Mentioned in 

Adopting the Verifier API in your iPhone app

## Discussion

Call this method to begin requesting data contained in a mobile document. This method displays a system-provided sheet with instructions on what the mobile document holder needs to do. This UI remains onscreen until the system reads the person’s mobile document, you cancel the task, or an error occurs.

Throws

This method throws a MobileDocumentReaderError if a mobile document request error occurs.

