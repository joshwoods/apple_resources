

- Quick Look
- QLPreviewingController
-  preparePreviewOfFile(at:completionHandler:) 

Instance Method

# preparePreviewOfFile(at:completionHandler:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

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

The URL of the file the user is about to preview.

`handler`  

The completion handler should be called whenever the view is ready to be displayed. A loading spinner will be shown until the handler is called. It can be called asynchronously after the method has returned.

## Discussion

Use this method to prepare the content of the view controller with the given file URL.

This method will be called only once. It will be called in the main thread before presenting the view controller. Heavy work potentially blocking the main thread should be avoided in this method.

