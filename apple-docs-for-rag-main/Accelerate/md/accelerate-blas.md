

- Accelerate
-  BLAS 

Structure

# BLAS

An enumeration that acts as a namespace for Swift overlays to BLAS.

iOSiPadOSMac CatalystmacOS 15.0+tvOSvisionOSwatchOS

``` source
struct BLAS
```

## Overview

The BLAS enumeration provides methods and structures that offer a Swift-friendly API for Basic Linear Algebra Subprograms (BLAS) and Linear Algebra PACKage (LAPACK) operations.

## Topics

### Setting the BLAS and LAPACK threading model

static var threadingModel: BLAS.ThreadingModel

The BLAS and LAPACK threading model.

struct ThreadingModel

Constants that describe the BLAS and LAPACK threading model.

## See Also

### Specifying the threading model

func BLASSetThreading(BLAS_THREADING) -> Int32

Sets the BLAS and LAPACK threading model.

func BLASGetThreading() -> BLAS_THREADING

Returns the current BLAS and LAPACK threading model.

struct BLAS_THREADING

Constants that describe the BLAS and LAPACK threading model.

