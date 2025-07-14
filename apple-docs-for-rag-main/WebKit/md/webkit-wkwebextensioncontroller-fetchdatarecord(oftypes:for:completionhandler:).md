

- WebKit
- WKWebExtensionController
-  fetchDataRecord(ofTypes:for:completionHandler:) 

Instance Method

# fetchDataRecord(ofTypes:for:completionHandler:)

Fetches a data record containing the given extension data types for a specific known web extension context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func fetchDataRecord(
    ofTypes dataTypes: Set,
    for extensionContext: WKWebExtensionContext,
    completionHandler: @escaping (WKWebExtension.DataRecord?) -> Void
)
```

``` source
@MainActor
func dataRecord(
    ofTypes dataTypes: Set,
    for extensionContext: WKWebExtensionContext
) async -> WKWebExtension.DataRecord?
```

## Parameters 

`dataTypes`  

The extension data types to fetch records for.

`extensionContext`  

The specific web extension context to fetch records for.

`completionHandler`  

A block to invoke when the data record has been fetched.

## Discussion

Note

The extension does not need to be loaded to be included in the result.

