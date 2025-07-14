

- Quick Look Thumbnailing
- QLThumbnailReply
-  init(imageFileURL:) 

Initializer

# init(imageFileURL:)

Creates a new thumbnail for a custom file type using a file at the given URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init(imageFileURL fileURL: URL)
```

## Parameters 

`fileURL`  

The URL to the file that is used as the thumbnail.

## Return Value

An initialized reply object for a requested thumbnail.

## Discussion

The image is scaled down to fit the provided size by the QLFileThumbnailRequest if necessary.

## See Also

### Creating a Thumbnail

convenience init(contextSize: CGSize, currentContextDrawing: () -> Bool)

Creates a new thumbnail for a custom file type in the current context.

convenience init(contextSize: CGSize, drawing: (CGContext) -> Bool)

Creates a new thumbnail for a custom file type in the given context.

