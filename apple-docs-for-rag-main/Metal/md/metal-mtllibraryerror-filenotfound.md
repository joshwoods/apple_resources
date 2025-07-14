

- Metal
- MTLLibraryError
-  fileNotFound 

Type Property

# fileNotFound

Metal couldn’t find the Metal source file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static var fileNotFound: MTLLibraryError.Code { get }
```

## See Also

### Errors

static var unsupported: MTLLibraryError.Code

Metal couldn’t support the requested action.

static var `internal`: MTLLibraryError.Code

The action caused an internal error.

static var compileFailure: MTLLibraryError.Code

The library or function failed to compile.

static var compileWarning: MTLLibraryError.Code

The library or function compiled successfully but generated warnings.

static var functionNotFound: MTLLibraryError.Code

Metal couldn’t find the specified Metal function.

