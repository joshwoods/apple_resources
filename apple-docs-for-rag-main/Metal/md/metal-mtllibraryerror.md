

- Metal
-  MTLLibraryError 

Structure

# MTLLibraryError

Metal errors related to libraries.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
struct MTLLibraryError
```

## Topics

### Errors

static var unsupported: MTLLibraryError.Code

Metal couldn’t support the requested action.

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

### Error Domain

static var errorDomain: String

The error domain used by Metal when returning library or function creation errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Error codes for Metal library errors.

let MTLLibraryErrorDomain: String

The error domain for Metal libraries.

