

- Metal
- MTLDevice
-  makeLibrary(data:) 

Instance Method

# makeLibrary(data:)

Creates a Metal library instance that contains the functions in a precompiled Metal library.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func makeLibrary(data: DispatchData) throws -> any MTLLibrary
```

## Parameters 

`data`  

The data from a precompiled Metal library. For more information, see Building a Shader Library by Precompiling Source Files.

## Return Value

A new MTLLibrary instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

Use this method if your application manages its own archiving system for libraries — for example, if your app uses a single file that contains several libraries.

Note

This is a Swift default implementation for the makeLibrary(data:) method.

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

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor) throws -> any MTLLibrary

Synchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor, completionHandler: MTLNewLibraryCompletionHandler)

Asynchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(data: dispatch_data_t) throws -> any MTLLibrary

Creates a Metal library instance from a dispatch-data instance that contains the functions in a precompiled Metal library.

**Required** Default implementation provided.

typealias MTLNewLibraryCompletionHandler

A completion handler signature a method calls when it finishes creating a Metal library.

func makeLibrary(filepath: String) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in the Metal library file at a file path.

**Required**

Deprecated

