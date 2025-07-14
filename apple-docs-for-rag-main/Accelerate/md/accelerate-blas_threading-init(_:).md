

- Accelerate
- BLAS_THREADING
-  init(\_:) 

Initializer

# init(\_:)

Creates a threading model constant.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(_ rawValue: UInt32)
```

## Parameters 

`rawValue`  

A raw unsigned-integer value.

## See Also

### Specifying a threading model

init(rawValue: UInt32)

Creates a threading model constant with an unsigned-integer value.

var rawValue: UInt32

The raw value that represents the threading model.

var BLAS_THREADING_MULTI_THREADED: BLAS_THREADING

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

var BLAS_THREADING_SINGLE_THREADED: BLAS_THREADING

A constant that specifies BLAS and LAPACK execute on a single thread only.

var BLAS_THREADING_MAX_OPTIONS: BLAS_THREADING

