

- AVFoundation
- Photo capture
- AVPortraitEffectsMatte
-  Extracting Portrait Effects Matte Image Data from a Photo 

Article

# Extracting Portrait Effects Matte Image Data from a Photo

Check for portrait effects matte metadata in existing images.

## Overview

The portrait effects matte is stored in the image file alongside the depth data auxiliary image. You can load, view, and edit the portrait effects matte as a high-level object called an AVPortraitEffectsMatte, analogous to AVDepthData. This mirrors traditional depth map access using AVDepthData in its technique to get the elementary auxiliary image bits out of the file.

### Load and View a Matting Image from File

Load the portrait effects matte by using Image I/O to extract an auxiliary image of type kCGImageAuxiliaryDataTypePortraitEffectsMatte. Convert this auxiliary image to an auxiliary information dictionary, which contains the matte as metadata of class CGImageMetadata. Generate the portrait effects matte object, AVPortraitEffectsMatte, by passing the dictionary to init(fromDictionaryRepresentation:). From this object, you can generate a CIImage object to bring the image into viewable forms, like UIImage.

- Swift
- Objective-C

```
func portraitEffectsMatteImage(at path: String) -> UIImage? {
    let bundlePath = Bundle.main.bundlePath
    let fileURL = URL(fileURLWithPath: bundlePath).appendingPathComponent(path)

    guard let source = CGImageSourceCreateWithURL(fileURL as CFURL, nil),
          let auxiliaryInfoDict = CGImageSourceCopyAuxiliaryDataInfoAtIndex(source, 0, kCGImageAuxiliaryDataTypePortraitEffectsMatte) as? [AnyHashable: Any] else { return nil }

    // Create a portrait effects matte from the auxiliary information.
    if let matteData = try? AVPortraitEffectsMatte(fromDictionaryRepresentation: auxiliaryInfoDict),
       let matteCIImage = CIImage(portaitEffectsMatte: matteData) {
        // Return a matte image by using the core image representation.
        return UIImage(ciImage: matteCIImage)
    }
    return nil
}
```

```
- (UIImage*) portraitEffectsMatteImageAtPath: (NSString*)path
{
    // Convert image path to a file URL:
    NSString* bundlePath = [NSBundle mainBundle].bundlePath;
    NSString* filePath = [bundlePath stringByAppendingPathComponent:path];
    CFURLRef urlRef = CFBridgingRetain([NSURL fileURLWithPath:filePath]);

    // Get reference to the image data:
    CGImageSourceRef source = CGImageSourceCreateWithURL(urlRef, nil);

    // Query for auxiliary data of specific type:
    CFDictionaryRef auxiliaryInfoDict = CGImageSourceCopyAuxiliaryDataInfoAtIndex(source, 0, kCGImageAuxiliaryDataTypePortraitEffectsMatte);

    NSDictionary* auxDataDictionary = (__bridge NSDictionary*)auxiliaryInfoDict;
    if (auxDataDictionary) {
        AVPortraitEffectsMatte* matteData = [AVPortraitEffectsMatte portraitEffectsMatteFromDictionaryRepresentation:auxDataDictionary error:nil];

        // Load matte data into Core Image for conversion to UIImage:
        CIImage* matteCIImage = [CIImage imageWithPortaitEffectsMatte:matteData];
        return [UIImage imageWithCIImage:matteCIImage];
    }
    else {
        return nil;
    }
}
```

With this matte image, your app can:

- Access the uncompressed pixels of the portrait effects matte in memory.

- Create rotated or flipped derivative copies of the mask.

- Replace a pixel of the matte with one of your own, reflecting an effect you’re applying to the main image.

- Create a dictionary of elementary PEM parts suitable for writing to a file using Image I/O’s CGImageDestination.

When decompressed, the matte images are natively L008 (kCVPixelFormatType_OneComponent8), which is an 8-bit one-component format where black is zero. Portrait effects matte images are not gamma corrected. They’re tagged with a linear transfer function, indicating that no color correction should be applied when working with them.

## See Also

### Examining a Portrait Effects Matte

var mattingImage: CVPixelBuffer

The portrait effects matte’s internal image, formatted as a pixel buffer.

var pixelFormatType: OSType

The pixel format type of this portrait effects matte’s internal image.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

A dictionary of primitive map information used for writing an image file with a portrait effects matte.

