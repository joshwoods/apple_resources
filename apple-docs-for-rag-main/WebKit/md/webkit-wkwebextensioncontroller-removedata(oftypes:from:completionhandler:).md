

- WebKit
- WKWebExtensionController
-  removeData(ofTypes:from:completionHandler:) 

Instance Method

# removeData(ofTypes:from:completionHandler:)

Removes extension data of the given types for the given data records.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    from dataRecords: [WKWebExtension.DataRecord],
    completionHandler: @escaping () -> Void
)
```

``` source
@MainActor
func removeData(
    ofTypes dataTypes: Set,
    from dataRecords: [WKWebExtension.DataRecord]
) async
```

## Parameters 

`dataTypes`  

The extension data types that should be removed.

`dataRecords`  

The extension data records to delete data from.

`completionHandler`  

A block to invoke when the data has been removed.

