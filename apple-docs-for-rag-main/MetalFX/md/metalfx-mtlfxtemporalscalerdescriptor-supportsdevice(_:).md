

- MetalFX
- MTLFXTemporalScalerDescriptor
-  supportsDevice(\_:) 

Type Method

# supportsDevice(\_:)

Returns a Boolean value that indicates whether the temporal scaler works with a GPU.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
class func supportsDevice(_ device: any MTLDevice) -> Bool
```

## Parameters 

`device`  

An MTLDevice instance that represents a GPU.

## See Also

### Checking a GPU device’s scaling support

class func supportedInputContentMinScale(device: any MTLDevice) -> Float

Returns the smallest temporal scaling factor the device supports as a floating-point value.

class func supportedInputContentMaxScale(device: any MTLDevice) -> Float

Returns the largest temporal scaling factor the device supports as a floating-point value.

