

- AVFoundation
- AVDepthData
-  availableDepthDataTypes 

Instance Property

# availableDepthDataTypes

The list of depth data formats to which you can convert this depth data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@nonobjc
var availableDepthDataTypes: [OSType] { get }
```

## Discussion

Use the converting(toDepthDataType:) method to obtain a converted depth data object using one of the types in this list.

## See Also

### Transforming and Processing

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a derivative depth data object by mirroring or rotating it to the specified orientation.

func converting(toDepthDataType: OSType) -> Self

Returns a derivative depth data object by converting the depth data map to the specified data type.

func replacingDepthDataMap(with: CVPixelBuffer) throws -> Self

Returns a derivative depth data object by replacing the depth data map.

