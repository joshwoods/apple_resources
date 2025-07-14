

- Quick Look Thumbnailing
- QLThumbnailProvider
-  provideThumbnail(for:\_:) 

Instance Method

# provideThumbnail(for:\_:)

Creates a thumbnail of a custom file type for a specific request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func provideThumbnail(
    for request: QLFileThumbnailRequest,
    _ handler: @escaping (QLThumbnailReply?, (any Error)?) -> Void
)
```

## Parameters 

`request`  

The request that contains information about the thumbnail that you need to provide, such as the URL to the file.

`handler`  

The completion handler to call when you finish creating a thumbnail. Call the completion handler with a QLThumbnailReply if you can provide a thumbnail or with an NSError if you can’t create a thumbnail.

The platform doesn’t draw a thumbnail if you pass an `error` to the handler or the `reply` is `nil.`

You can call the handler asynchronously after the method has returned.

`reply`  
The object containing information about the thumbnail image that the platform uses to draw the thumbnail.

`error`  
An error object that indicates why the thumbnail generation failed, or `nil` if the thumbnail generation succeeded.

## Mentioned in 

Providing Thumbnails of Your Custom File Types

## Discussion

To provide a thumbnail for a custom file type, subclass QLThumbnailProvider, implement this method, and return a QLThumbnailReply that either contains a drawing block or the URL to an image file.

