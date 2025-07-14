

- Quick Look UI
- QLPreviewingController
-  providePreview(for:completionHandler:) 

Instance Method

# providePreview(for:completionHandler:)

Prepares the preview of a file identified within a file preview request.

macOS 12.0+

``` source
optional func providePreview(
    for request: QLFilePreviewRequest,
    completionHandler handler: @escaping (QLPreviewReply?, (any Error)?) -> Void
)
```

``` source
optional func providePreview(for request: QLFilePreviewRequest) async throws -> QLPreviewReply
```

## Parameters 

`request`  

The file preview request that identifies the content to preview.

`handler`  

The closure to call with a doc://com.apple.documentation/documentation/quicklook/qlpreviewreply for the system to display as the preview.

## See Also

### Instance Methods

func preparePreviewOfFile(at: URL, completionHandler: ((any Error)?) -> Void)

Prepares the preview of a file at the specified file’s URL.

func preparePreviewOfSearchableItem(identifier: String, queryString: String?, completionHandler: ((any Error)?) -> Void)

Prepares the preview for a file by using the data from Spotlight’s searchable item.

