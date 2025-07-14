

- Core Image
- CIKernel
-  makeKernels(source:) Deprecated

Type Method

# makeKernels(source:)

Creates and returns and array of `CIKernel` objects.

iOS 8.0–12.0DeprecatediPadOS 8.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func makeKernels(source string: String) -> [CIKernel]?
```

## Parameters 

`s`  

A program in the Core Image Kernel Language that contains one or more routines, each of which is marked using the `kernel` keyword.

## Return Value

An array of `CIKernel` objects. The array contains one `CIKernel` objects for each kernel routine in the supplied string. Each object in the array can be of class `CIKernel`, CIColorKernel, or CIWarpKernel depending on the corresponding routine specified in the Core Image Kernel Language source code string.

## Discussion

The Core Image Kernel Language is a dialect of the OpenGL Shading Language. See Core Image Kernel Language Reference and Core Image Programming Guide for more details.

## See Also

### Deprecated

init?(source: String)

Creates a single kernel object.

Deprecated

