

- AVFoundation
- AVDepthData
-  converting(toDepthDataType:) 

Instance Method

# converting(toDepthDataType:)

Returns a derivative depth data object by converting the depth data map to the specified data type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func converting(toDepthDataType depthDataType: OSType) -> Self
```

## Parameters 

`depthDataType`  

The data type to convert to. This value must be one of the formats present in the availableDepthDataTypes array.

## Return Value

A new, converted depth data object.

## Discussion

This method raises an exception if you pass an invalid `depthDataType` value.

## See Also

### Transforming and Processing

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a derivative depth data object by mirroring or rotating it to the specified orientation.

var availableDepthDataTypes: [OSType]

The list of depth data formats to which you can convert this depth data.

func replacingDepthDataMap(with: CVPixelBuffer) throws -> Self

Returns a derivative depth data object by replacing the depth data map.

