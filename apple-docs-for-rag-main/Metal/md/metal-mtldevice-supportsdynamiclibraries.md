

- Metal
- MTLDevice
-  supportsDynamicLibraries 

Instance Property

# supportsDynamicLibraries

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in compute pipelines.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var supportsDynamicLibraries: Bool { get }
```

**Required**

## See Also

### Creating Dynamic Shader Libraries

var supportsRenderDynamicLibraries: Bool

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in render pipelines.

**Required**

func makeDynamicLibrary(library: any MTLLibrary) throws -> any MTLDynamicLibrary

Creates a Metal dynamic library instance from a Metal library instance.

**Required**

func makeDynamicLibrary(url: URL) throws -> any MTLDynamicLibrary

Creates a Metal dynamic library instance that contains the functions in the Metal library file at a URL.

**Required**

enum Code

Error codes that Metal can generate when creating dynamic libraries.

let MTLDynamicLibraryDomain: String

The domain for Metal dynamic library errors.

