

- Quick Look UI
- QLPreviewingController
-  preparePreviewOfFile(at:completionHandler:) 

Instance Method

# preparePreviewOfFile(at:completionHandler:)

Prepares the preview of a file at the specified file’s URL.

macOS 10.10+

``` source
optional func preparePreviewOfFile(
    at url: URL,
    completionHandler handler: @escaping ((any Error)?) -> Void
)
```

``` source
optional func preparePreviewOfFile(at url: URL) async throws
```

## Parameters 

`url`  

The URL of the file to preview.

`handler`  

A completion handler that notifies the platform that a preview is available. The operating system shows a loading spinner, so call the handler as soon as possible. You can call the completion handler asynchronously after returning from the callback.

## Discussion

The operating system calls this method only once from the main thread before it presents the previewing controller. To avoid blocking the main thread, don’t perform long-running or resource-intensive work.

When preparing and displaying the view controller, avoid holding open a file descriptors while the user is previewing the file.

## See Also

### Instance Methods

func preparePreviewOfSearchableItem(identifier: String, queryString: String?, completionHandler: ((any Error)?) -> Void)

Prepares the preview for a file by using the data from Spotlight’s searchable item.

func providePreview(for: QLFilePreviewRequest, completionHandler: (QLPreviewReply?, (any Error)?) -> Void)

Prepares the preview of a file identified within a file preview request.

