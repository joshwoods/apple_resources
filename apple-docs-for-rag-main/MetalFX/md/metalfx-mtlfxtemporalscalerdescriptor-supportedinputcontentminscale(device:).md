

- MetalFX
- MTLFXTemporalScalerDescriptor
-  supportedInputContentMinScale(device:) 

Type Method

# supportedInputContentMinScale(device:)

Returns the smallest temporal scaling factor the device supports as a floating-point value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class func supportedInputContentMinScale(device: any MTLDevice) -> Float
```

## Parameters 

`device`  

The MTLDevice instance that represents a GPU.

## See Also

### Checking a GPU device’s scaling support

class func supportsDevice(any MTLDevice) -> Bool

Returns a Boolean value that indicates whether the temporal scaler works with a GPU.

class func supportedInputContentMaxScale(device: any MTLDevice) -> Float

Returns the largest temporal scaling factor the device supports as a floating-point value.

