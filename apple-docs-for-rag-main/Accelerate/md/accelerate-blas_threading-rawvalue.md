

- Accelerate
- BLAS_THREADING
-  rawValue 

Instance Property

# rawValue

The raw value that represents the threading model.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rawValue: UInt32
```

## See Also

### Specifying a threading model

init(UInt32)

Creates a threading model constant.

init(rawValue: UInt32)

Creates a threading model constant with an unsigned-integer value.

var BLAS_THREADING_MULTI_THREADED: BLAS_THREADING

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

var BLAS_THREADING_SINGLE_THREADED: BLAS_THREADING

A constant that specifies BLAS and LAPACK execute on a single thread only.

var BLAS_THREADING_MAX_OPTIONS: BLAS_THREADING

