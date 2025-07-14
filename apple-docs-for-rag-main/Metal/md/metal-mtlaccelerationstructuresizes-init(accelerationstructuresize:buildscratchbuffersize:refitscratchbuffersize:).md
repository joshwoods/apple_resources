

- Metal
- MTLAccelerationStructureSizes
-  init(accelerationStructureSize:buildScratchBufferSize:refitScratchBufferSize:) 

Initializer

# init(accelerationStructureSize:buildScratchBufferSize:refitScratchBufferSize:)

Creates an acceleration sizes instance with specific values.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    accelerationStructureSize: Int,
    buildScratchBufferSize: Int,
    refitScratchBufferSize: Int
)
```

## Parameters 

`accelerationStructureSize`  

The size of the acceleration structure, in bytes.

`buildScratchBufferSize`  

The amount of scratch memory, in bytes, the GPU devices needs to build the acceleration structure.

`refitScratchBufferSize`  

The amount of scratch memory, in bytes, the GPU device needs to refit the acceleration structure.

## See Also

### Creating an Acceleration Size Structure

init()

Creates an acceleration sizes instance with default values.

