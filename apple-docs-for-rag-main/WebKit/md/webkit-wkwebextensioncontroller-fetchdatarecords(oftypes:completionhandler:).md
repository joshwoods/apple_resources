

- WebKit
- WKWebExtensionController
-  fetchDataRecords(ofTypes:completionHandler:) 

Instance Method

# fetchDataRecords(ofTypes:completionHandler:)

Fetches data records containing the given extension data types for all known extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func fetchDataRecords(
    ofTypes dataTypes: Set,
    completionHandler: @escaping ([WKWebExtension.DataRecord]) -> Void
)
```

``` source
@MainActor
func dataRecords(ofTypes dataTypes: Set) async -> [WKWebExtension.DataRecord]
```

## Parameters 

`dataTypes`  

The extension data types to fetch records for.

`completionHandler`  

A block to invoke when the data records have been fetched.

## Discussion

Note

The extension does not need to be loaded to be included in the result.

