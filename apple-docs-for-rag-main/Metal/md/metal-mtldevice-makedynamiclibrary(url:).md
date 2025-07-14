

- Metal
- MTLDevice
-  makeDynamicLibrary(url:) 

Instance Method

# makeDynamicLibrary(url:)

Creates a Metal dynamic library instance that contains the functions in the Metal library file at a URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeDynamicLibrary(url: URL) throws -> any MTLDynamicLibrary
```

**Required**

## Parameters 

`url`  

A URL to a Metal library file (ending in `.metallib`).

## Return Value

A new MTLDynamicLibrary instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Mentioned in 

Compiling and Linking Metal Dynamic Libraries

## See Also

### Creating Dynamic Shader Libraries

var supportsDynamicLibraries: Bool

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in compute pipelines.

**Required**

var supportsRenderDynamicLibraries: Bool

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in render pipelines.

**Required**

func makeDynamicLibrary(library: any MTLLibrary) throws -> any MTLDynamicLibrary

Creates a Metal dynamic library instance from a Metal library instance.

**Required**

enum Code

Error codes that Metal can generate when creating dynamic libraries.

let MTLDynamicLibraryDomain: String

The domain for Metal dynamic library errors.

