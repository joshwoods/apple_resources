

- Core Image
- CIKernel
-  init(source:) Deprecated

Initializer

# init(source:)

Creates a single kernel object.

iOS 8.0–12.0DeprecatediPadOS 8.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init?(source string: String)
```

## Parameters 

`string`  

A program in the Core Image Kernel Language that contains a single routine marked using the `kernel` keyword.

## Return Value

A new kernel object. The class of the returned object can be `CIKernel`, CIColorKernel, or CIWarpKernel depending on the type of routine specified in the Core Image Kernel Language source code string.

## Discussion

The Core Image Kernel Language is a dialect of the OpenGL Shading Language. See Core Image Kernel Language Reference and Core Image Programming Guide for more details.

## See Also

### Deprecated

class func makeKernels(source: String) -> [CIKernel]?

Creates and returns and array of `CIKernel` objects.

Deprecated

### Related Documentation

Core Image Programming Guide

Core Image Kernel Language Reference

