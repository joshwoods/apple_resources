

- MediaExtension
-  Video decoder entitlement 

Article

# Video decoder entitlement

Include an entitlement to indicate your extension is a MediaExtension video decoder.

## Overview

MediaExtension video decoders must include an special entitlement key with a Boolean value set to true. To add the entitlement key in Xcode, follow these steps:

1.  Select the build target for your format reader extension

2.  Go to the Signing & Capabilities tab

3.  Click + to add a new capability

4.  Choose Media Extension Video Decoder from the list

The entitlement key is `com.apple.developer.mediaextension.videodecoder` and it must have a Boolean value set to true. A developer provisioning profile will be needed to use this entitlement.

## See Also

### Video decoders

protocol MEVideoDecoder

A protocol that defines the requirements for a video decoder.

protocol MEVideoDecoderExtension

A protocol that defines a factory to create new video decoders for a codec type that the extension implements.

class MEDecodeFrameOptions

An object that guides the video decoder operation on a per-frame basis.

class MEVideoDecoderPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

Video decoder property list dictionary

Include a property list dictionary to describe a video decoder.

