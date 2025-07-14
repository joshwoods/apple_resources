

- Video Toolbox
-  VTPixelRotationSession 

API Collection

# VTPixelRotationSession

An object that rotates source pixel buffers to destination pixel buffers.

## Overview

To create a rotation session, call VTPixelRotationSessionCreate(_:_:). Optionally configure the session by calling VTSessionSetProperty(_:key:value:).

To transfer pixels call VTPixelRotationSessionRotateImage(_:_:_:).

When you’re done with the session, call CFRelease to tear it down and release your object reference.

## Topics

### Managing a Session

func VTPixelRotationSessionCreate(CFAllocator?, UnsafeMutablePointer&lt;VTPixelRotationSession?>) -> OSStatus

Creates a session to rotate images between pixel buffers.

func VTPixelRotationSessionInvalidate(VTPixelRotationSession)

Tears down a pixel rotation session.

### Configuring a Session

Pixel Rotation Properties

Properties used to configure a VideoToolbox pixel rotation session.

### Rotating an Image

func VTPixelRotationSessionRotateImage(VTPixelRotationSession, CVPixelBuffer, CVPixelBuffer) -> OSStatus

Rotates a source pixel buffer and writes the output to the destination pixel buffer.

### Inspecting the Type Identifier

func VTPixelRotationSessionGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for the rotation session.

### Data Types

class VTPixelRotationSession

A reference to a pixel rotation session.

## See Also

### Transformation

VTPixelTransferSession

An object converts video data from source pixel buffers to destination pixel buffers.

