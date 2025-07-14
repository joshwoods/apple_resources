

- Group Activities
- GroupSessionJournal
- GroupSessionJournal.Attachment
-  loadMetadata(of:) 

Instance Method

# loadMetadata(of:)

Downloads the metadata for the attachment asynchronously and delivers it as the type you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func loadMetadata(of: MetadataType.Type) async throws -> MetadataType where MetadataType : Decodable, MetadataType : Encodable
```

## Parameters 

`of`  

The type for your attachment’s custom metadata. This type must match the one added with the attachment.

## Return Value

The custom metadata object for the attachment.

## Discussion

Use this function to retrieve any metadata you included with the attachment. You might use this metadata to retrieve app-specific details that aren’t part of the item’s intrinsic data format.

## See Also

### Downloading the attachment data

func load&lt;AttachmentType>(AttachmentType.Type) async throws -> AttachmentType

Downloads the attachment data and asynchronously delivers it as the type you specify.

