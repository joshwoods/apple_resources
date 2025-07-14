

- Quick Look
-  QLThumbnailCreate(\_:\_:\_:\_:) Deprecated

Function

# QLThumbnailCreate(\_:\_:\_:\_:)

Returns a thumbnail that’s generated in the background.

macOS 10.6–15.0Deprecated

``` source
func QLThumbnailCreate(
    _ allocator: CFAllocator!,
    _ url: CFURL!,
    _ maxThumbnailSize: CGSize,
    _ options: CFDictionary!
) -> Unmanaged!
```

Deprecated

Use QLThumbnailGenerationRequest in QuickLookThumbnailing to generate thumbnails.

## Parameters 

`allocator`  

The allocator to use to create the thumbnail.

`url`  

The URL of the document that you want to request a thumbnail for.

`maxThumbnailSize`  

The maximum size in points for the thumbnail image.

`options`  

Optional hints for creating a thumbnail image. Available options are kQLThumbnailOptionScaleFactorKey and kQLThumbnailOptionIconModeKey.

## Return Value

A generated thumbnail of the file at the provided `url`.

## See Also

### Creating thumbnails

func QLThumbnailImageCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;CGImage>!

Creates a thumbnail image for the specified file.

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

func QLThumbnailIsCancelled(QLThumbnail!) -> Bool

Returns whether the creation of the thumbnail was canceled.

Deprecated

