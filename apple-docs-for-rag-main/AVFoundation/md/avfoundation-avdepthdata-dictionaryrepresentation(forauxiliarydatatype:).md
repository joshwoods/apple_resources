

- AVFoundation
- AVDepthData
-  dictionaryRepresentation(forAuxiliaryDataType:) 

Instance Method

# dictionaryRepresentation(forAuxiliaryDataType:)

Returns a dictionary representation of the depth data suitable for writing into an image file.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func dictionaryRepresentation(forAuxiliaryDataType outAuxDataType: AutoreleasingUnsafeMutablePointer?) -> [AnyHashable : Any]?
```

## Parameters 

`outAuxDataType`  

On output, either kCGImageAuxiliaryDataTypeDisparity or kCGImageAuxiliaryDataTypeDepth, depending on the depth data’s type.

## Discussion

When using `CGImageDestination` functions to write depth data (along with image data) to a HEIF, JPEG, or DNG file, you can use this method to obtain a dictionary of primitive depth map information, then use the CGImageDestinationAddAuxiliaryDataInfo(_:_:_:) function to embed that data into the output file.

## See Also

### Creating Depth Data

convenience init(fromDictionaryRepresentation: [AnyHashable : Any]) throws

Creates a depth data object from depth information such as that found in an image file.

