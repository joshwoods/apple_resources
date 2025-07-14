

- Metal
-  MTLSamplePosition 

Structure

# MTLSamplePosition

A subpixel sample position for use in multisample antialiasing (MSAA).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLSamplePosition
```

## Mentioned in 

Positioning Samples Programmatically

## Overview

Subpixel sample positions are in a 16 x 16 grid across a pixel. Each subsample position’s x and y values are in 1/16 increments in the floating-point range `[0.0, 15.0/16.0)`. The pixel’s origin point `(0,0)` is at the top-left corner.

See Positioning Samples Programmatically for the details on working with subpixels.

## Topics

### Initializers

init()

Returns a new sample position on a subpixel grid.

init(x: Float, y: Float)

Returns a new sample position on a subpixel grid at specified coordinates.

### Instance Properties

var x: Float

The x position of the sample on the subpixel grid.

var y: Float

The y position of the sample on the subpixel grid.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Texture Samplers

Creating and Sampling Textures

Load image data into a texture and apply it to a quadrangle.

protocol MTLSamplerState

An object that defines how a texture should be sampled.

class MTLSamplerDescriptor

An object that you use to configure a texture sampler.

