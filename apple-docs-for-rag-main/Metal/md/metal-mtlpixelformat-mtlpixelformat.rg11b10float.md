

- Metal
- MTLPixelFormat
-  MTLPixelFormat.rg11b10Float 

Case

# MTLPixelFormat.rg11b10Float

32-bit format with floating-point color components, 11 bits each for red and green and 10 bits for blue.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case rg11b10Float
```

## Discussion

The components have no sign bit. The 10-bit float has 5 bits of mantissa and 5 bits of exponent. The 11-bit floats have 6 bits of mantissa and 5 bits of exponent.

## See Also

### Packed 32-Bit Pixel Formats

case bgr10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit blue, 10-bit green, 10-bit red, and 2-bit alpha.

case rgb10a2Unorm

A 32-bit packed pixel format with four normalized unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rgb10a2Uint

A 32-bit packed pixel format with four unsigned integer components: 10-bit red, 10-bit green, 10-bit blue, and 2-bit alpha.

case rgb9e5Float

Packed 32-bit format with floating-point color components: 9 bits each for RGB and 5 bits for an exponent shared by RGB, packed into 32 bits.

