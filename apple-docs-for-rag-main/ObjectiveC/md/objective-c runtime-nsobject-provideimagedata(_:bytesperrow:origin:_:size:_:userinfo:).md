

- Objective-C Runtime
- NSObject
-  provideImageData(\_:bytesPerRow:origin:\_:size:\_:userInfo:) 

Instance Method

# provideImageData(\_:bytesPerRow:origin:\_:size:\_:userInfo:)

Supplies data to a `CIImage` object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func provideImageData(
    _ data: UnsafeMutableRawPointer,
    bytesPerRow rowbytes: Int,
    origin x: Int,
    _ y: Int,
    size width: Int,
    _ height: Int,
    userInfo info: Any?
)
```

## Parameters 

`data`  

A pointer to image data. Note that `data[0]` refers to the first byte of the requested subimage, not the larger image buffer.

`rowbytes`  

The number of bytes per row.

`x`  

The x origin of the image data.

`y`  

The y origin of the image data.

`width`  

The width of the image data.

`height`  

The height of the image data.

`info`  

User supplied data, which is optional.

## Discussion

You can supply the image provider to these methods of the `CIImage` class:

- imageWithImageProvider:size::format:colorSpace:options: to create a CIImage object from image data

- init(imageProvider:size:_:format:colorSpace:options:) to initialize an existing CIImage with data

You initialize the given bitmap with the subregion specified by the arguments `x`, `y`, `width`, and `height`. The subregion uses the local coordinate space of the image, with the origin at the upper-left corner of the image. If you change the virtual memory mapping of the buffer specified by the `data` argument (such as by using `vm_copy` to modify it), the behavior is undefined.

That this callback always requests the full image data regardless of what is actually visible. All of the image is loaded or none of it is. The exception is when you create a tiled image by specifying the `kCIImageProviderTileSize` option. In this case, only the needed tiles are requested.

## See Also

### Related Documentation

Core Image Programming Guide

