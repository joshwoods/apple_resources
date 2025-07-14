

- Metal
- MTLAccelerationStructureCommandEncoder
-  refit(sourceAccelerationStructure:descriptor:destinationAccelerationStructure:scratchBuffer:scratchBufferOffset:options:) 

Instance Method

# refit(sourceAccelerationStructure:descriptor:destinationAccelerationStructure:scratchBuffer:scratchBufferOffset:options:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func refit(
    sourceAccelerationStructure: any MTLAccelerationStructure,
    descriptor: MTLAccelerationStructureDescriptor,
    destinationAccelerationStructure: (any MTLAccelerationStructure)?,
    scratchBuffer: (any MTLBuffer)?,
    scratchBufferOffset: Int,
    options: MTLAccelerationStructureRefitOptions = []
)
```

**Required**

