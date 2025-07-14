

- Metal
- MTLLibraryError
-  compileFailure 

Type Property

# compileFailure

The library or function failed to compile.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
static var compileFailure: MTLLibraryError.Code { get }
```

## See Also

### Errors

static var unsupported: MTLLibraryError.Code

Metal couldn’t support the requested action.

static var `internal`: MTLLibraryError.Code

The action caused an internal error.

static var compileWarning: MTLLibraryError.Code

The library or function compiled successfully but generated warnings.

static var fileNotFound: MTLLibraryError.Code

Metal couldn’t find the Metal source file.

static var functionNotFound: MTLLibraryError.Code

Metal couldn’t find the specified Metal function.

