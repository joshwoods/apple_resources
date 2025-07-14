

- Metal
- MTLAccelerationStructureCommandEncoder
-  copyAndCompact(sourceAccelerationStructure:destinationAccelerationStructure:) 

Instance Method

# copyAndCompact(sourceAccelerationStructure:destinationAccelerationStructure:)

Encodes a command to compact an acceleration structure’s data and copy it into a different acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func copyAndCompact(
    sourceAccelerationStructure: any MTLAccelerationStructure,
    destinationAccelerationStructure: any MTLAccelerationStructure
)
```

**Required**

## Parameters 

`sourceAccelerationStructure`  

The source acceleration structure.

`destinationAccelerationStructure`  

The destination acceleration structure.

## Discussion

The source and destination acceleration structures must not overlap in memory. The destination acceleration structure must be at least as large as the compacted size of the source acceleration structure, which you obtain by using the writeCompactedSize(accelerationStructure:buffer:offset:) method.

If the source acceleration structure contains references to other acceleration structures, the copied acceleration structure references the same child structures.

## See Also

### Copying an Acceleration Structure

func copy(sourceAccelerationStructure: any MTLAccelerationStructure, destinationAccelerationStructure: any MTLAccelerationStructure)

Encodes a command to copy the data from one acceleration structure to another.

**Required**

func writeCompactedSize(accelerationStructure: any MTLAccelerationStructure, buffer: any MTLBuffer, offset: Int)

Encodes a command to calculate the compacted size of an acceleration structure.

**Required**

func writeCompactedSize(accelerationStructure: any MTLAccelerationStructure, buffer: any MTLBuffer, offset: Int, sizeDataType: MTLDataType)

Encodes a command to calculate the compacted size of an acceleration structure, taking into account the size of the output data.

**Required**

