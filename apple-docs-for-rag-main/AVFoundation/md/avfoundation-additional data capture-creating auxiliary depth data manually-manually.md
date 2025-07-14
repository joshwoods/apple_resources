

- AVFoundation
- Additional data capture
-  Creating Auxiliary Depth Data Manually 

Article

# Creating Auxiliary Depth Data Manually

Generate a depth image and attach it to your own image.

## Overview

iOS Portrait Mode generates a depth map and attaches it to the image as auxiliary metadata, but for custom effects, you can generate your own auxiliary depth image, one not taken with iOS Portrait Mode or another depth-enabled capture device. This article shows you how to generate this map and attach it to your image.

### Convert Pixel Values into a Compatible Floating-Point Format

The depth image is a single-component image that must be converted per-pixel from grayscale pixel values (`0` = black to `1` = white, zNear to zFar) to either depth (in meters) or disparity (in 1/meters). Then adjust these values to fit your desired floating-point format.

The supported pixel formats for disparity or depth images are:

- `kCVPixelFormatType_DisparityFloat16 = 'hdis'`: An IEEE754-2008 binary16 (half float), describing the normalized shift when comparing two images. Units are 1/meters: (pixelShift / (pixelFocalLength \* baselineInMeters))

- `kCVPixelFormatType_DisparityFloat32 = 'fdis'`: An IEEE754-2008 binary32 float, describing the normalized shift when comparing two images. Units are 1/meters: (pixelShift / (pixelFocalLength \* baselineInMeters))

- `kCVPixelFormatType_DepthFloat16 = 'hdep'`: An IEEE754-2008 binary16 (half float), describing the depth (distance to an object) in meters

- `kCVPixelFormatType_DepthFloat32 = 'fdep'`: An IEEE754-2008 binary32 float, describing the depth (distance to an object) in meters

Load the grayscale image into a CVPixelBuffer. Load its base address, attained via CVPixelBufferLockBaseAddress(_:_:), as data (CFData) and pass it as the kCGImageAuxiliaryDataInfoData value into a dictionary (CFDictionary).

### Parse Metadata Dictionaries

The format of the dictionary is documented in `CGImageSource.h`. Access this dictionary with CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:). The dictionary supports JPEG, HEIF, and DNG images. The CFDictionary contains auxiliary data in the following format:

- kCGImageAuxiliaryDataInfoData → Depth data (CFData)

- kCGImageAuxiliaryDataInfoDataDescription → Depth data description (CFDictionary: See below for more details.)

- kCGImageAuxiliaryDataInfoMetadata → Optional metadata (CGImageMetadata)

CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:) returns `nil` if the image doesn’t contain `auxiliaryImageDataType` data.

The value for key kCGImageAuxiliaryDataInfoDataDescription is a CFDictionary that you populate to tell the image system how to interpret the depth map. It can contain the following depth data parameters:

- kCGImagePropertyPixelFormat → One of the Core Video `CVPixelBuffer.h` depth or disparity formats

- kCGImagePropertyWidth and kCGImagePropertyHeight → Pixel dimensions

- kCGImagePropertyBytesPerRow → The number of bytes per row in the depth map

### Attach Your Custom Depth Map to an Image

Attach the depth or disparity dictionary to an image as follows:

1.  Create AVDepthData with init(fromDictionaryRepresentation:), passing in the depth or disparity dictionary.

2.  Create the image destination.

3.  Create the image, using helper methods from Image I/O.

```
// Add an image to the destination.
CGImageDestinationAddImage(cgImageDestination, renderedCGImage, attachments)  

// Use AVDepthData to get the auxiliary data dictionary.         
var auxDataType :NSString? 
let auxData = depthData.dictionaryRepresentation(forAuxiliaryDataType: &auxDataType)  

// Add auxiliary data to the image destination. 
CGImageDestinationAddAuxiliaryDataInfo(cgImageDestination, auxDataType!, auxData! as CFDictionary)  

if CGImageDestinationFinalize(cgImageDestination) {  
   return data as Data
}  
```

## See Also

### Depth data capture

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Capturing depth using the LiDAR camera

Access the LiDAR camera on supporting devices to capture precise depth data.

AVCamFilter: Applying Filters to a Capture Stream

Render a capture stream with rose-colored filtering and depth effects.

Streaming Depth Data from the TrueDepth Camera

Visualize depth data in 2D and 3D from the TrueDepth camera.

Enhancing Live Video by Leveraging TrueDepth Camera Data

Apply your own background to a live capture feed streamed from the front-facing TrueDepth camera.

class AVCaptureDepthDataOutput

A capture output that records scene depth information on compatible camera devices.

class AVDepthData

A container for per-pixel distance or disparity information captured by compatible camera devices.

class AVCameraCalibrationData

Information about the camera characteristics used to capture images and depth data.

