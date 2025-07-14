

- Core Image
- CIKernel
-  init(functionName:fromMetalLibraryData:) 

Initializer

# init(functionName:fromMetalLibraryData:)

Creates a single kernel object using a Metal Shading Language (MSL) kernel function.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
convenience init(
    functionName name: String,
    fromMetalLibraryData data: Data
) throws
```

## Parameters 

`functionName`  

The name of the function in the Metal shading language.

`fromMetalLibraryData`  

A metallib file compiled with the Core Image Standard Library.

## Discussion

This method allows you to use MSL as the shader language for a Core Image kernel. Since MSL based kernels are precompiled, initializing them is faster than their than Core Image Kernel Language (CIKL) counterparts and Xcode can provide error diagnostics during development rather than at runtime. MSL is a more modern language than CIKL, and you can write shader code that uses arrays, structs and matrices.

MSL based kernels still support concatenation and tiling and can work in the same filter graph as traditional CIKL kernels.

### Specifying Compiler and Linker Options

To use MSL as the shader language for a CIKernel, you must specify some options in Xcode under the *Build Settings* tab of your project's target. The first option you need to specify is an `-fcikernel` flag in the Other Metal Compiler Flags option. The second is to add a user-defined setting with a key called `MTLLINKER_FLAGS` with a value of `-cikernel:`

Figure 1 Specifying Compiler and Linker Options in Xcode.

### Creating a General Kernel in Swift

The following code shows how you can create a general kernel based on a Metal function named `myKernel`.

The first step is to create a `Data` object that represents the the default Metal library. If you have built this in Xcode, it will be called `default.metallib` and can be loaded using the Bundle type's `url` method.

Using the representation of the Metal library and the function name `myKernel`, you initialize a CIKernel.

guard
    let url = Bundle.main.url(forResource: &quot;default&quot;, withExtension: &quot;metallib&quot;),
    let data = try? Data(contentsOf: url) else {
    fatalError(&quot;Unable to get metallib&quot;)
}

guard let generalKernel = try? CIKernel(functionName: &quot;myKernel&quot;, fromMetalLibraryData: data) else {
    fatalError(&quot;Unable to create CIKernel from myKernel&quot;)
}

The code to create general, color, warp and blend filters is identical.

### Metal Shading Language Extensions

Core Image provides a set of language extensions to MSL in `CIKernelMetalLib.h`. These extensions include three new data types for working with images: `sampler` (for accessing the input image), `sample_t` (represents a single color sample from the input image), and `destination `(for accessing the output image). The extensions also include convenience functions such as color conversion and premultiply / unpremultiply.

Whereas in CIKL, you typically called global functions when working with, for example, coordinates and samples, these functions are implemented as member functions on the new types.

The following table shows a summary of CIKL global functions and their equivalent MSL functions.

|  | Core Image Kernel Language | Metal Shading Language |
|----|----|----|
| Get destination coordinate | `destCoord()` | `dest.coord()` |
| Transform coordinate to sampler space | `samplerTransform(src, p)` | `src.transform(p)` |
| Get destination coordinate in sampler space | `samplerCoord(src)` | `src.coord()` |
| Sample from source image | `sample(src, p)` | `src.sample(p)` |
| Get extent of source image | `samplerExtent(src)` | `src.extent()` |

## See Also

### Creating a Kernel Using Metal Shading Language

init(functionName: String, fromMetalLibraryData: Data, outputPixelFormat: CIFormat)

Creates a single kernel object using a Metal Shading Language kernel function with optional pixel format.

class func kernelNames(fromMetalLibraryData: Data) -> [String]

Return an array of strings containing the names of all of the kernels contained in the Metal library.

class func kernels(withMetalString: String) -> [CIKernel]

Load kernels from a Metal language string.

