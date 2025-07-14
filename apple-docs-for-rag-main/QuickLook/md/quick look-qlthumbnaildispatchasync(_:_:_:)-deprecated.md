

- Quick Look
-  QLThumbnailDispatchAsync(\_:\_:\_:) Deprecated

Function

# QLThumbnailDispatchAsync(\_:\_:\_:)

Creates a thumbnail in the background on the provided background queue.

macOS 10.6–15.0Deprecated

``` source
func QLThumbnailDispatchAsync(
    _ thumbnail: QLThumbnail!,
    _ queue: dispatch_queue_t!,
    _ completion: (() -> Void)!
)
```

Deprecated

Use QLThumbnailGenerator in QuickLookThumbnailing to generate thumbnails.

## Parameters 

`thumbnail`  

The thumbnail to compute.

`queue`  

The queue that’s used to create the thumbnail.

`completion`  

The completion block that’s called when the thumbnail is created. The completion block is always called, even if the thumbnail computation is canceled.

## See Also

### Creating thumbnails

func QLThumbnailImageCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;CGImage>!

Creates a thumbnail image for the specified file.

Deprecated

func QLThumbnailCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;QLThumbnail>!

Returns a thumbnail that’s generated in the background.

Deprecated

func QLThumbnailCancel(QLThumbnail!)

Cancels the computation of the thumbnail.

Deprecated

func QLThumbnailCopyDocumentURL(QLThumbnail!) -> Unmanaged&lt;CFURL>!

Returns the URL of the document that you’re requesting a thumbnail for.

Deprecated

func QLThumbnailCopyImage(QLThumbnail!) -> Unmanaged&lt;CGImage>!

Returns a thumbnail image.

Deprecated

func QLThumbnailCopyOptions(QLThumbnail!) -> Unmanaged&lt;CFDictionary>!

Returns the options for the requested thumbnail.

Deprecated

func QLThumbnailGetContentRect(QLThumbnail!) -> CGRect

Returns the rectangle of the provided thumbnail image that represents the content of the document.

Deprecated

func QLThumbnailGetMaximumSize(QLThumbnail!) -> CGSize

Returns the maximum allowed size for the provided thumbnail image.

Deprecated

func QLThumbnailGetTypeID() -> CFTypeID

Returns the type identifier for the thumbnail’s opaque type.

Deprecated

func QLThumbnailIsCancelled(QLThumbnail!) -> Bool

Returns whether the creation of the thumbnail was canceled.

Deprecated

