

- Metal
- MTLLibraryError
-  unsupported 

Type Property

# unsupported

Metal couldn’t support the requested action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
static var unsupported: MTLLibraryError.Code { get }
```

## Discussion

For example, the requested library file has improper formatting, or the requested library isn’t accessible.

## See Also

### Errors

static var `internal`: MTLLibraryError.Code

The action caused an internal error.

static var compileFailure: MTLLibraryError.Code

The library or function failed to compile.

static var compileWarning: MTLLibraryError.Code

The library or function compiled successfully but generated warnings.

static var fileNotFound: MTLLibraryError.Code

Metal couldn’t find the Metal source file.

static var functionNotFound: MTLLibraryError.Code

Metal couldn’t find the specified Metal function.

