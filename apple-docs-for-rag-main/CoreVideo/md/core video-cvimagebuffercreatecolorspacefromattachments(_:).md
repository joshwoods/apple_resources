

- Core Video
-  CVImageBufferCreateColorSpaceFromAttachments(\_:) 

Function

# CVImageBufferCreateColorSpaceFromAttachments(\_:)

Attempts to create a Core Graphics color space from the image buffer’s attachments that you specify.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func CVImageBufferCreateColorSpaceFromAttachments(_ attachments: CFDictionary) -> Unmanaged?
```

## Parameters 

`attachments`  

The dictionary of attachments for an image buffer, which you can obtain by calling CVBufferCopyAttachments(_:_:) on the image buffer.

## Return Value

A CGColorSpace object that represents the color space of the image buffer, or nil if the dictionary doesn’t contain the information required to create a CGColorSpace instance.

## Discussion

To generate a CGColorSpace instance, the attachments dictionary needs to include values for either:

1.  kCVImageBufferICCProfileKey

2.  kCVImageBufferColorPrimariesKey, kCVImageBufferTransferFunctionKey, kCVImageBufferYCbCrMatrixKey, and possibly kCVImageBufferGammaLevelKey

Use CGColorSpaceRelease to release the color space when you’re done with it.

