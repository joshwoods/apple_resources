

- Quick Look
-  QLThumbnailImageCreate(\_:\_:\_:\_:) Deprecated

Function

# QLThumbnailImageCreate(\_:\_:\_:\_:)

Creates a thumbnail image for the specified file.

macOS 10.6–15.0Deprecated

``` source
func QLThumbnailImageCreate(
    _ allocator: CFAllocator!,
    _ url: CFURL!,
    _ maxThumbnailSize: CGSize,
    _ options: CFDictionary!
) -> Unmanaged!
```

Deprecated

Use QuickLookThumbnailing to generate thumbnails for files.

## Parameters 

`allocator`  

The allocator to use to create the thumbnail image.

`url`  

The URL of the file to create a thumbnail image for.

`maxThumbnailSize`  

The maximum desired size of the thumbnail image.

`options`  

A dictionary of options that affect the creation of the thumbnail image. You can use kQLThumbnailOptionIconModeKey and kQLThumbnailOptionScaleFactorKey as options.

## Return Value

The thumbnail image, or `NULL` if Quick Look doesn’t support this file type.

## Discussion

This function doesn’t supplant the use of Icon Services by apps to get generic file icons and custom icons stored in the metadata fork of files.

### Special Considerations

This function is thread-safe, so you can call it from any thread. However, because it’s synchronous, you should generally call it in a background thread.

## See Also

### Creating thumbnails

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

func QLThumbnailIsCancelled(QLThumbnail!) -> Bool

Returns whether the creation of the thumbnail was canceled.

Deprecated

