

- Core Image
- CIColorKernel
-  apply(extent:arguments:) 

Instance Method

# apply(extent:arguments:)

Creates a new image using the kernel and specified arguments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func apply(
    extent: CGRect,
    arguments args: [Any]
) -> CIImage?
```

## Parameters 

`extent`  

The extent of the output image.

`args`  

An array of arguments to pass to the kernel routine. The type of each object in the array must be compatible with the corresponding parameter declared in the kernel routine source code. For details, see Core Image Kernel Language Reference.

## Return Value

A new image object describing the result of applying the kernel.

## Discussion

This method is analogous to the CIFilter method apply(_:arguments:options:), but it does not require construction of a `CIFilter` object, and it allows you to specify a callback for determining the kernel’s region of interest as a block or closure. As with the similar `CIFilter` method, calling this method does not execute the kernel code—filters and their kernel code are evaluated only when rendering a final output image.

