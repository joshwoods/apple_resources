

- Metal
- MTLLibraryError
-  MTLLibraryError.Code 

Enumeration

# MTLLibraryError.Code

Error codes for Metal library errors.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case unsupported

Metal couldn’t support the requested action.

case `internal`

The action caused an internal error.

case compileFailure

The library or function failed to compile.

case compileWarning

The library or function compiled successfully but generated warnings.

case fileNotFound

Metal couldn’t find the Metal source file.

case functionNotFound

Metal couldn’t find the specified Metal function.

case unsupported

Metal couldn’t support the requested action.

case `internal`

The action caused an internal error.

case compileFailure

The library or function failed to compile.

case compileWarning

The library or function compiled successfully but generated warnings.

case fileNotFound

Metal couldn’t find the Metal source file.

case functionNotFound

Metal couldn’t find the specified Metal function.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct MTLLibraryError

Metal errors related to libraries.

let MTLLibraryErrorDomain: String

The error domain for Metal libraries.

