

- Accelerate
-  BLAS_THREADING_MAX_OPTIONS 

Global Variable

# BLAS_THREADING_MAX_OPTIONS

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var BLAS_THREADING_MAX_OPTIONS: BLAS_THREADING { get }
```

## See Also

### Specifying a threading model

init(UInt32)

Creates a threading model constant.

init(rawValue: UInt32)

Creates a threading model constant with an unsigned-integer value.

var rawValue: UInt32

The raw value that represents the threading model.

var BLAS_THREADING_MULTI_THREADED: BLAS_THREADING

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

var BLAS_THREADING_SINGLE_THREADED: BLAS_THREADING

A constant that specifies BLAS and LAPACK execute on a single thread only.

