

- Metal
- MTLBlitOption
-  rowLinearPVRTC 

Type Property

# rowLinearPVRTC

A blit option that copies PVRTC data between a texture and a buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+macOS 11.0+tvOS 9.0+visionOS 1.0+

``` source
static var rowLinearPVRTC: MTLBlitOption { get }
```

## Discussion

The PowerVR Texture Compression (PVRTC) format arranges blocks linearly in memory in row-major order, similar to other compressed texture formats. You can pass this option to some methods that copy data between a buffer and a texture, including the following:

- copy(from:sourceOffset:sourceBytesPerRow:sourceBytesPerImage:sourceSize:to:destinationSlice:destinationLevel:destinationOrigin:options:)

- copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:)

