

- Core Image
- CIImageProcessorKernel
-  roi(forInput:arguments:outputRect:) 

Type Method

# roi(forInput:arguments:outputRect:)

Method to override for determining specific region of input image required to process in rendering a specified region of the output image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class func roi(
    forInput input: Int32,
    arguments: [String : Any]?,
    outputRect: CGRect
) -> CGRect
```

## Parameters 

`input`  

Index of the input image.

`arguments`  

Dictionary of arguments mapping keys such as `"thresholdValue"` to their values.

`outputRect`  

Rectangle defining the area of output that must be rendered.

## Return Value

Rectangle defining the region of the input image over which the kernel should execute.

## Discussion

Override this method if your image processor needs to work with a larger or smaller region of interest in the input image than each corresponding region of the output image (for example, a blur filter, which samples several input pixels for each output pixel).

This will be called one or more times per render to determine the portion of the input images needed to render a given `outputRect` of the output. This will not be called if there are 0 input images.

The default implementation simply returns `outputRect`.

