

- Metal
- MTLDataType
-  MTLDataType.rgb9e5Float 

Case

# MTLDataType.rgb9e5Float

A packed 32-bit format with three color components, each of which is a 9-bit floating-point value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
case rgb9e5Float
```

## Discussion

The color components are in RGBA order, which stands for red, green, blue, and alpha. The red, green, and blue components each have 9 bits, and the alpha component has 5 bits.

## See Also

### 32-bit Pixel Format Types

case rgba8Snorm

An ordinary pixel with four components, each of which is an 8-bit, normalized, signed integer value.

case rgba8Unorm

An ordinary pixel with four components, each of which is an 8-bit, normalized, unsigned integer value.

case rgba8Unorm_srgb

An ordinary pixel with four components, each of which is an 8-bit, normalized, unsigned integer value in the sRGB color space.

case rg16Snorm

An ordinary pixel with two components, each of which is a 16-bit, normalized, signed integer value.

case rg16Unorm

An ordinary pixel with two components, each of which is a 16-bit, normalized, unsigned integer value.

case rgb10a2Unorm

A packed 32-bit format with three color components, each of which is a 10-bit, normalized, unsigned integer value.

case rg11b10Float

A packed 32-bit format with three floating-point color components, two of which are 11-bit values, and one is a 10-bit value.

