

- Metal
- MTLRasterizationRateMap
-  parameterDataSizeAndAlign 

Instance Property

# parameterDataSizeAndAlign

The size and alignment requirements to contain the coordinate transformation information in this rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var parameterDataSizeAndAlign: MTLSizeAndAlign { get }
```

**Required**

## Mentioned in 

Scaling Variable Rasterization Rate Content

## Discussion

To convert coordinate values inside your shader, pass the rate map data into the shader in a MTLBuffer object. The place in the buffer where you store the parameter information must have at least the size and alignment provided by this property.

## See Also

### Obtaining Coordinate Transformation Data

func copyParameterData(buffer: any MTLBuffer, offset: Int)

Copies the parameter data into the provided buffer.

**Required**

