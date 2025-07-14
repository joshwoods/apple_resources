

- Media Player
- MPMediaItemArtwork
-  image(at:) 

Instance Method

# image(at:)

Returns the artwork image for an item at the given size.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

**macOS**

``` source
func image(at size: CGSize) -> NSImage?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func image(at size: CGSize) -> UIImage?
```

## Parameters 

`size`  

The size, in points, for the new UIImage object.

## Return Value

The artwork at the requested size.

## Discussion

The returned image is the smallest available image that’s at least as large as the requested size.

## See Also

### Related Documentation

iPod Library Access Programming Guide

### Using a media item image

var bounds: CGRect

The maximum size, in points, of the image associated with the media item artwork.

