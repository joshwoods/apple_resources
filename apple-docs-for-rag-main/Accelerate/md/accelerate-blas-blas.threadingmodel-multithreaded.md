

- Accelerate
- BLAS
- BLAS.ThreadingModel
-  multiThreaded 

Type Property

# multiThreaded

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

iOSiPadOSMac CatalystmacOS 15.0+tvOSvisionOSwatchOS

``` source
static let multiThreaded: BLAS.ThreadingModel
```

## See Also

### Specifying a threading model

static let singleThreaded: BLAS.ThreadingModel

A constant that specifies BLAS and LAPACK execute on a single thread only.

