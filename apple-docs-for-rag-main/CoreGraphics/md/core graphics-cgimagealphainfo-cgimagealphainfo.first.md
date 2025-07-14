

- Core Graphics
- CGImageAlphaInfo
-  CGImageAlphaInfo.first 

Case

# CGImageAlphaInfo.first

The alpha component is stored in the most significant bits of each pixel. For example, non-premultiplied ARGB.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case first
```

## See Also

### Constants

case last

The alpha component is stored in the least significant bits of each pixel. For example, non-premultiplied RGBA.

case none

There is no alpha channel.

case noneSkipFirst

There is no alpha channel. If the total size of the pixel is greater than the space required for the number of color components in the color space, the most significant bits are ignored.

case alphaOnly

There is no color data, only an alpha channel.

case noneSkipLast

There is no alpha channel.

case premultipliedFirst

The alpha component is stored in the most significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied ARGB.

case premultipliedLast

The alpha component is stored in the least significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied RGBA.

