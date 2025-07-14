

- Video Toolbox
-  VTPixelTransferSession 

API Collection

# VTPixelTransferSession

An object converts video data from source pixel buffers to destination pixel buffers.

## Overview

A pixel transfer session supports the copying and/or conversion of images from source pixel buffers to destination pixel buffers. The basic workflow used when working with a pixel transfer session is as follows:

1.  Create a pixel transfer session by calling VTPixelTransferSessionCreate(allocator:pixelTransferSessionOut:).

2.  Optionally, configure the session with your desired Pixel Transfer Properties by calling VTSessionSetProperty(_:key:value:) or VTSessionSetProperties(_:propertyDictionary:).

3.  Transfer images by calling VTPixelTransferSessionTransferImage(_:from:to:).

4.  When you finish with the pixel transfer session, call VTPixelTransferSessionInvalidate(_:) to tear it down, and CFRelease to free its memory.

## Topics

### Creating Sessions

func VTPixelTransferSessionCreate(allocator: CFAllocator?, pixelTransferSessionOut: UnsafeMutablePointer&lt;VTPixelTransferSession?>) -> OSStatus

Creates a session for transferring images between Core Video image buffers that hold pixels in main memory.

### Configuring Sessions

Pixel Transfer Properties

Properties used to configure a VideoToolbox pixel transfer session.

### Converting Image Data

func VTPixelTransferSessionTransferImage(VTPixelTransferSession, from: CVPixelBuffer, to: CVPixelBuffer) -> OSStatus

Copies and/or converts an image from one pixel buffer to another.

### Inspecting Sessions

func VTPixelTransferSessionGetTypeID() -> CFTypeID

Retrieves the Core Foundation type identifier for the pixel transfer session.

### Ending Sessions

func VTPixelTransferSessionInvalidate(VTPixelTransferSession)

Tears down a pixel transfer session.

### Data Types

class VTPixelTransferSession

A reference to a VideoToolbox pixel transfer session.

## See Also

### Transformation

VTPixelRotationSession

An object that rotates source pixel buffers to destination pixel buffers.

