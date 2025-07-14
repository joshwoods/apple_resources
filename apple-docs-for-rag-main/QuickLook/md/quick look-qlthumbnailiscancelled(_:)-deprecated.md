

- Quick Look
-  QLThumbnailIsCancelled(\_:) Deprecated

Function

# QLThumbnailIsCancelled(\_:)

Returns whether the creation of the thumbnail was canceled.

macOS 10.6–15.0Deprecated

``` source
func QLThumbnailIsCancelled(_ thumbnail: QLThumbnail!) -> Bool
```

Deprecated

Use QuickLookThumbnailing for thumbnails.

## Parameters 

`thumbnail`  

The thumbnail to create.

## Return Value

A `Boolean` value that indicates whether the creation of the thumbnail was canceled.

## See Also

### Creating thumbnails

func QLThumbnailImageCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;CGImage>!

Creates a thumbnail image for the specified file.

Deprecated

func QLThumbnailCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;QLThumbnail>!

Returns a thumbnail that’s generated in the background.

Deprecated

func QLThumbnailDispatchAsync(QLThumbnail!, dispatch_queue_t!, (() -> Void)!)

Creates a thumbnail in the background on the provided background queue.

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

