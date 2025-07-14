

- BrowserEngineKit
- BETextInput
-  requestDocumentContext(\_:completionHandler:) 

Instance Method

# requestDocumentContext(\_:completionHandler:)

Gathers context about the current document for the system

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func requestDocumentContext(
    _ request: BETextDocumentRequest,
    completionHandler: @escaping (BETextDocumentContext) -> Void
)
```

``` source
func requestDocumentContext(_ request: BETextDocumentRequest) async -> BETextDocumentContext
```

**Required**

