

- Core Image
- CIKernel
-  kernels(withMetalString:) 

Type Method

# kernels(withMetalString:)

Load kernels from a Metal language string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class func kernels(withMetalString source: String) throws -> [CIKernel]
```

## Parameters 

`source`  

A string containing the progam in Metal language.

## Return Value

An array of CIKernel objects.

## See Also

### Creating a Kernel Using Metal Shading Language

init(functionName: String, fromMetalLibraryData: Data)

Creates a single kernel object using a Metal Shading Language (MSL) kernel function.

init(functionName: String, fromMetalLibraryData: Data, outputPixelFormat: CIFormat)

Creates a single kernel object using a Metal Shading Language kernel function with optional pixel format.

class func kernelNames(fromMetalLibraryData: Data) -> [String]

Return an array of strings containing the names of all of the kernels contained in the Metal library.

