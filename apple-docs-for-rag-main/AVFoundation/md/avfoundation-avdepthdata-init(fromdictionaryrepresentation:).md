

- AVFoundation
- AVDepthData
-  init(fromDictionaryRepresentation:) 

Initializer

# init(fromDictionaryRepresentation:)

Creates a depth data object from depth information such as that found in an image file.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
convenience init(fromDictionaryRepresentation imageSourceAuxDataInfoDictionary: [AnyHashable : Any]) throws
```

## Parameters 

`imageSourceAuxDataInfoDictionary`  

A dictionary of primitive depth-related information, in the format provided by the CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:) function.

## Mentioned in 

Creating Auxiliary Depth Data Manually

## Discussion

When using `CGImageSource` functions to read from a HEIF, JPEG, or DNG file containing depth data (as well as image data), you can use the CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:) function to load primitive depth map information, then use this initializer to create an AVDepthData object, as shown below.

```
- (nullable AVDepthData *)depthDataFromImageData:(nonnull NSData *)imageData {
   AVDepthData *depthData = nil;

    CGImageSourceRef imageSource = CGImageSourceCreateWithData((CFDataRef)imageData, NULL);
   if (imageSource) {
       NSDictionary *auxDataDictionary = (__bridge NSDictionary *)CGImageSourceCopyAuxiliaryDataInfoAtIndex(imageSource, 0, kCGImageAuxiliaryDataTypeDisparity);
       if (auxDataDictionary) {
           depthData = [AVDepthData depthDataFromDictionaryRepresentation:auxDataDictionary error:NULL];
       }

       CFRelease(imageSource);
   }

    return depthData;
}
```

## See Also

### Creating Depth Data

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

Returns a dictionary representation of the depth data suitable for writing into an image file.

