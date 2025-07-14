

- Metal
- MTLDevice
-  makeLibrary(stitchedDescriptor:) 

Instance Method

# makeLibrary(stitchedDescriptor:)

Synchronously creates a Metal library from the function stitching graphs in a descriptor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func makeLibrary(stitchedDescriptor descriptor: MTLStitchedLibraryDescriptor) throws -> any MTLLibrary
```

**Required**

## Parameters 

`descriptor`  

An MTLStitchedLibraryDescriptor instance.

## Return Value

A new MTLLibrary instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

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

func makeLibrary(source: String, options: MTLCompileOptions?, completionHandler: MTLNewLibraryCompletionHandler)

Asynchronously creates a Metal library instance by compiling the functions in a source string.

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

