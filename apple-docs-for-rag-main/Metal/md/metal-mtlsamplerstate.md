

- Metal
-  MTLSamplerState 

Protocol

# MTLSamplerState

An object that defines how a texture should be sampled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLSamplerState : NSObjectProtocol
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

Adding Mipmap Filtering to Samplers

## Overview

The MTLSamplerState protocol defines the interface for a lightweight object used to encode how a shader or compute kernel should sample a texture. To create a sampler state object:

1.  Create a MTLSamplerDescriptor object.

2.  Set the desired properties of the sampler descriptor, including filtering options, addressing modes, maximum anisotropy, and level-of-detail parameters.

3.  Call the makeSamplerState(descriptor:) method of the MTLDevice object.

(Your app does not define a class that implements the MTLSamplerState protocol.)

You can either release the MTLSamplerDescriptor object or modify its property values and reuse it to create more MTLSamplerState objects. The descriptor’s properties are only used during object creation; once created the behavior of a sampler state object is fixed and cannot be changed.

## Topics

### Identifying the Sampler

var device: any MTLDevice

The device object that created the sampler.

**Required**

var label: String?

A string that identifies the sampler.

**Required**

### Instance Properties

var gpuResourceID: MTLResourceID

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Texture Samplers

Creating and Sampling Textures

Load image data into a texture and apply it to a quadrangle.

class MTLSamplerDescriptor

An object that you use to configure a texture sampler.

struct MTLSamplePosition

A subpixel sample position for use in multisample antialiasing (MSAA).

