

- Metal
- MTLAccelerationStructureCommandEncoder
-  refit(sourceAccelerationStructure:descriptor:destinationAccelerationStructure:scratchBuffer:scratchBufferOffset:) 

Instance Method

# refit(sourceAccelerationStructure:descriptor:destinationAccelerationStructure:scratchBuffer:scratchBufferOffset:)

Updates an acceleration structure with new geometry or instance data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func refit(
    sourceAccelerationStructure: any MTLAccelerationStructure,
    descriptor: MTLAccelerationStructureDescriptor,
    destinationAccelerationStructure: (any MTLAccelerationStructure)?,
    scratchBuffer: (any MTLBuffer)?,
    scratchBufferOffset: Int
)
```

**Required**

## Parameters 

`sourceAccelerationStructure`  

The source acceleration structure.

`descriptor`  

A description of the updated acceleration structure.

`destinationAccelerationStructure`  

The destination to write the new acceleration structure to. Pass the same acceleration structure or `nil` to refit the structure in place.

`scratchBuffer`  

A buffer used to hold data while building the acceleration structure.

`scratchBufferOffset`  

An offset, in bytes, in the scratch buffer where the scratch memory starts.

## Discussion

Use refitting to update an acceleration structure when you’ve made small changes to the underlying geometry. Refitting can be much faster than rebuilding an acceleration structure from scratch. However, ray-tracing performance may degrade, based on how many changes you made to the geometry data.

You can’t use refitting to add or remove geometry in the acceleration structure.

If the source and destination acceleration structures are not the same, they must not overlap in memory. The destination acceleration structure and the scratch buffer must have enough space in memory to hold the acceleration structure data. Call the accelerationStructureSizes(descriptor:) method on the Metal device object to get the required space. If you’ve already compacted the source structure, the destination must be at least as large as the compacted size of the source acceleration structure.

