

- Core Image
- CIImageProcessorKernel
-  formatForInput(at:) 

Type Method

# formatForInput(at:)

Method to override for returning the image processing kernel's input pixel format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class func formatForInput(at input: Int32) -> CIFormat
```

## Parameters 

`input`  

Index of this image processor in a multi-step workflow.

## Return Value

Core Image pixel format CIFormat constant revealing the processor's input pixel format.

## Discussion

Override this method and the outputFormat property getter to customize your processor's input and output pixel format.

The format must be one of CIFormat: BGRA8, RGBAh, RGBAf, or R8. If the outputFormat is 0, then the output will be a supported format that best matches the rendering context's workingFormat.

