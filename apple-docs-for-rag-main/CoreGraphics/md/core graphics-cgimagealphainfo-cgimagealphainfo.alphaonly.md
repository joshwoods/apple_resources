

- Core Graphics
- CGImageAlphaInfo
-  CGImageAlphaInfo.alphaOnly 

Case

# CGImageAlphaInfo.alphaOnly

There is no color data, only an alpha channel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case alphaOnly
```

## See Also

### Constants

case first

The alpha component is stored in the most significant bits of each pixel. For example, non-premultiplied ARGB.

case last

The alpha component is stored in the least significant bits of each pixel. For example, non-premultiplied RGBA.

case none

There is no alpha channel.

case noneSkipFirst

There is no alpha channel. If the total size of the pixel is greater than the space required for the number of color components in the color space, the most significant bits are ignored.

case noneSkipLast

There is no alpha channel.

case premultipliedFirst

The alpha component is stored in the most significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied ARGB.

case premultipliedLast

The alpha component is stored in the least significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied RGBA.

