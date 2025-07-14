

- Accelerate
- BLAS
-  BLAS.ThreadingModel 

Structure

# BLAS.ThreadingModel

Constants that describe the BLAS and LAPACK threading model.

iOSiPadOSMac CatalystmacOS 15.0+tvOSvisionOSwatchOS

``` source
struct ThreadingModel
```

## Overview

Use the threading model constants to specify whether BLAS and LAPACK operations run in a single thread or multiple threads. Specify the single-threaded model if your app uses its own threading mechanism.

## Topics

### Specifying a threading model

static let multiThreaded: BLAS.ThreadingModel

A constant that specifies that the Accelerate framework decides whether BLAS and LAPACK execute on single or multiple threads.

static let singleThreaded: BLAS.ThreadingModel

A constant that specifies BLAS and LAPACK execute on a single thread only.

## Relationships

### Conforms To

- Equatable
- RawRepresentable

## See Also

### Setting the BLAS and LAPACK threading model

static var threadingModel: BLAS.ThreadingModel

The BLAS and LAPACK threading model.

