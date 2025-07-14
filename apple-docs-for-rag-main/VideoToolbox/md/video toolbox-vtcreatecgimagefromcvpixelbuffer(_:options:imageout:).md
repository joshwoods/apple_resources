

- Video Toolbox
-  VTCreateCGImageFromCVPixelBuffer(\_:options:imageOut:) 

Function

# VTCreateCGImageFromCVPixelBuffer(\_:options:imageOut:)

Creates a Core Graphics bitmap image or image mask using the provided pixel buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.2+visionOS 1.0+

``` source
func VTCreateCGImageFromCVPixelBuffer(
    _ pixelBuffer: CVPixelBuffer,
    options: CFDictionary?,
    imageOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`pixelBuffer`  

A pixel buffer to use as the image data source for the CGImage.

`options`  

No options are currently supported. Pass `NULL` for this argument.

`imageOut`  

Pointer to an address to receive the newly created CGImage.

## Discussion

This routine creates a CGImage representation of the image data contained in the provided CVPixelBuffer. The source `CVPixelBuffer` may be retained for the lifetime of the `CGImage`. Changes to the `CVPixelBuffer` after making this call (other than releasing it) will have undefined results.

Not all `CVPixelBuffer` pixel formats support conversion into a `CGImage-`compatible pixel format.

