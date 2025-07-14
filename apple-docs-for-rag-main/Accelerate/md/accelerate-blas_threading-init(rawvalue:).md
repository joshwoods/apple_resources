

- Accelerate
- BLAS_THREADING
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a threading model constant with an unsigned-integer value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(rawValue: UInt32)
```

## Parameters 

`rawValue`  

A raw unsigned-integer value.

## See Also

### Specifying a threading model

init(UInt32)

Creates a threading model constant.

var rawValue: UInt32

The raw value that represents the threading model.

var BLAS_THREADING_MULTI_THREADED: BLAS_THREADING

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

var BLAS_THREADING_SINGLE_THREADED: BLAS_THREADING

A constant that specifies BLAS and LAPACK execute on a single thread only.

var BLAS_THREADING_MAX_OPTIONS: BLAS_THREADING

