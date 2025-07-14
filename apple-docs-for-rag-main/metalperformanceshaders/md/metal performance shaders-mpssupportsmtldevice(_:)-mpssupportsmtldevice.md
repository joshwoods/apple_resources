

- Metal Performance Shaders
-  MPSSupportsMTLDevice(\_:) 

Function

# MPSSupportsMTLDevice(\_:)

Determines whether the Metal Performance Shaders framework supports a Metal device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
func MPSSupportsMTLDevice(_ device: (any MTLDevice)?) -> Bool
```

## Parameters 

`device`  

A valid Metal device.

## Return Value

- `true` if the device is supported.

- `false` if the device is not supported.

## Discussion

For a full listing of Metal Performance Shaders feature set support, see Feature Availability.

