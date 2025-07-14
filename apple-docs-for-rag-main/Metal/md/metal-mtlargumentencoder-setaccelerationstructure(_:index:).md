

- Metal
- MTLArgumentEncoder
-  setAccelerationStructure(\_:index:) 

Instance Method

# setAccelerationStructure(\_:index:)

Encodes a reference to an acceleration structure into the argument buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setAccelerationStructure(
    _ accelerationStructure: (any MTLAccelerationStructure)?,
    index: Int
)
```

**Required**

## Parameters 

`accelerationStructure`  

An acceleration structure the method encodes.

`index`  

The index of an acceleration structure within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

