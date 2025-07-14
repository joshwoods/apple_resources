

- Group Activities
- GroupSessionJournal
- GroupSessionJournal.Attachment
-  load(\_:) 

Instance Method

# load(\_:)

Downloads the attachment data and asynchronously delivers it as the type you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func load(_ attachmentType: AttachmentType.Type) async throws -> AttachmentType where AttachmentType : Transferable
```

## Parameters 

`attachmentType`  

The type you use to interpret the data. An app typically uploads and downloads a single type of data for an activity. For more information about defining your types, see Transferable.

## Return Value

A requested type that contains the downloaded information.

## Discussion

Use this function to retrieve the file or data another participant provides. The method asynchronously retrieves and decodes the data, returning it as the requested type. If the requested type isn’t available, the method throws an error.

## See Also

### Downloading the attachment data

func loadMetadata&lt;MetadataType>(of: MetadataType.Type) async throws -> MetadataType

Downloads the metadata for the attachment asynchronously and delivers it as the type you specify.

