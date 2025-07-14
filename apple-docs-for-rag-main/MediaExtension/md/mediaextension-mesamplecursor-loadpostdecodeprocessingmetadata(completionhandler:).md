

- MediaExtension
- MESampleCursor
-  loadPostDecodeProcessingMetadata(completionHandler:) 

Instance Method

# loadPostDecodeProcessingMetadata(completionHandler:)

Asynchronously loads a dictionary that represents frame level metadata for post decode processing.

macOS 14.0+

``` source
optional func loadPostDecodeProcessingMetadata(completionHandler: @escaping ([String : any Sendable]?, (any Error)?) -> Void)
```

``` source
optional func postDecodeProcessingMetadata() async throws -> [String : any Sendable]
```

## Parameters 

`completionHandler`  

The handler that will be invoked when the method completes.

## Discussion

This method should provide either a valid NSDictionary or `nil`. If the method fails, the NSError will contain error information.

The post decode processing metadata could either be contained in the media asset primary file or be located in a separate related “sidecar” file. If contained in a separate file with a different extension, that file extension should be included in the EXAppExtensionAttributes and UTExportedTypeDeclarations dictionaries in the MediaExtension format reader `Info.plist`. The metadata returned should contain sequence level metadata for post decode processing, along with optional frame level metadata if present.

Typically the metadata returned by this method is delivered to the video decoder through sample buffer attachments.

