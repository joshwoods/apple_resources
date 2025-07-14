

- Metal
- MTLDevice
-  makeLibrary(source:options:completionHandler:) 

Instance Method

# makeLibrary(source:options:completionHandler:)

Asynchronously creates a Metal library instance by compiling the functions in a source string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeLibrary(
    source: String,
    options: MTLCompileOptions?,
    completionHandler: @escaping MTLNewLibraryCompletionHandler
)
```

``` source
func makeLibrary(
    source: String,
    options: MTLCompileOptions?
) async throws -> any MTLLibrary
```

**Required**

## Parameters 

`source`  

A string that contains source code for one or more Metal functions. For information about writing source in Metal Shading Language (MSL), see the Metal Shading Language Specification.

`options`  

An MTLCompileOptions instance that affects the compilation of the source code in the string.

`completionHandler`  

A Swift closure or an Objective-C block the method calls when the library finishes loading.

## Mentioned in 

Minimizing the Binary Size of a Shader Library

## Discussion

Because there’s no search path to find other functions, the source may only import the Metal default library.

## See Also

### Creating Shader Libraries

func makeDefaultLibrary() -> (any MTLLibrary)?

Creates a Metal library instance that contains the functions from your app’s default Metal library.

**Required**

func makeDefaultLibrary(bundle: Bundle) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in a bundle’s default Metal library.

**Required**

func makeLibrary(URL: URL) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in the Metal library file at a URL.

**Required**

func makeLibrary(source: String, options: MTLCompileOptions?) throws -> any MTLLibrary

Synchronously creates a Metal library instance by compiling the functions in a source string.

**Required**

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor) throws -> any MTLLibrary

Synchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor, completionHandler: MTLNewLibraryCompletionHandler)

Asynchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(data: DispatchData) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in a precompiled Metal library.

func makeLibrary(data: dispatch_data_t) throws -> any MTLLibrary

Creates a Metal library instance from a dispatch-data instance that contains the functions in a precompiled Metal library.

**Required** Default implementation provided.

typealias MTLNewLibraryCompletionHandler

A completion handler signature a method calls when it finishes creating a Metal library.

func makeLibrary(filepath: String) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in the Metal library file at a file path.

**Required**

Deprecated

