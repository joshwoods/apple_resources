

- Accelerate
- BLAS
- BLAS.ThreadingModel
-  singleThreaded 

Type Property

# singleThreaded

A constant that specifies BLAS and LAPACK execute on a single thread only.

iOSiPadOSMac CatalystmacOS 15.0+tvOSvisionOSwatchOS

``` source
static let singleThreaded: BLAS.ThreadingModel
```

## See Also

### Specifying a threading model

static let multiThreaded: BLAS.ThreadingModel

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

