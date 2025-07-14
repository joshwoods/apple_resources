

- Metal
- MTLPixelFormat
-  MTLPixelFormat.bgr10a2Unorm 

Case

# MTLPixelFormat.bgr10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit blue, 10-bit green, 10-bit red, and 2-bit alpha.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
case bgr10a2Unorm
```

## Discussion

Pixel data is stored in blue, green, red, and alpha order, from least significant bit to most significant bit.

On devices with a wide color display, use this format instead of MTLPixelFormat.bgra8Unorm to reduce banding artifacts in your displayed content.

## See Also

### Packed 32-Bit Pixel Formats

case rgb10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rgb10a2Uint

A 32-bit packed pixel format with four unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rg11b10Float

32-bit format with floating-point color components, 11 bits each for red and green and 10 bits for blue.

case rgb9e5Float

Packed 32-bit format with floating-point color components: 9 bits each for RGB and 5 bits for an exponent shared by RGB, packed into 32 bits.

