

- Metal
- MTLRasterizationRateMap
-  copyParameterData(buffer:offset:) 

Instance Method

# copyParameterData(buffer:offset:)

Copies the parameter data into the provided buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func copyParameterData(
    buffer: any MTLBuffer,
    offset: Int
)
```

**Required**

## Parameters 

`buffer`  

The buffer object to copy the data into. It must have a MTLStorageMode.shared storage mode, and there must be enough room in the buffer to store the data.

`offset`  

The location in the buffer to copy the data to. The offset must be a multiple of the parameter alignment.

## Discussion

To convert coordinate values inside your shader, pass the rate map data into the shader in a MTLBuffer object. Use the parameterDataSizeAndAlign property to determine the size and alignment requirements for the buffer.

## See Also

### Obtaining Coordinate Transformation Data

var parameterDataSizeAndAlign: MTLSizeAndAlign

The size and alignment requirements to contain the coordinate transformation information in this rate map.

**Required**

