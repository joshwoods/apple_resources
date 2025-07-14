

- Metal
- MTLDevice
-  supportsFamily(\_:) 

Instance Method

# supportsFamily(\_:)

Returns a Boolean value that indicates whether the GPU device supports the feature set of a specific GPU family.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func supportsFamily(_ gpuFamily: MTLGPUFamily) -> Bool
```

**Required**

## Parameters 

`gpuFamily`  

A MTLGPUFamily instance.

## Mentioned in 

Improving your game’s graphics performance and settings

Setting Resource Storage Modes

Choosing a Resource Storage Mode for Intel and AMD GPUs

## See Also

### Checking a GPU Device’s Feature Support

enum MTLGPUFamily

Represents the functionality for families of GPUs.

func supportsFeatureSet(MTLFeatureSet) -> Bool

Returns a Boolean value that indicates whether the GPU device supports a specific feature set.

**Required**

Deprecated

enum MTLFeatureSet

The device feature sets that define specific platform, hardware, and software configurations.

Deprecated

