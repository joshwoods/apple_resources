

- Core Image
- CIKernel
-  kernelNames(fromMetalLibraryData:) 

Type Method

# kernelNames(fromMetalLibraryData:)

Return an array of strings containing the names of all of the kernels contained in the Metal library.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func kernelNames(fromMetalLibraryData data: Data) -> [String]
```

## Parameters 

`data`  

Contents of the Metal library.

## Return Value

An Array of strings containing the names of the kernels.

## See Also

### Creating a Kernel Using Metal Shading Language

init(functionName: String, fromMetalLibraryData: Data)

Creates a single kernel object using a Metal Shading Language (MSL) kernel function.

init(functionName: String, fromMetalLibraryData: Data, outputPixelFormat: CIFormat)

Creates a single kernel object using a Metal Shading Language kernel function with optional pixel format.

class func kernels(withMetalString: String) -> [CIKernel]

Load kernels from a Metal language string.

