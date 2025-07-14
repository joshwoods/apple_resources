

- Accelerate
-  BLAS_THREADING 

Structure

# BLAS_THREADING

Constants that describe the BLAS and LAPACK threading model.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BLAS_THREADING
```

## Overview

Use the threading model constants to specify whether BLAS and LAPACK operations run in a single thread or multiple threads. Specify the single-threaded model if your app uses its own threading mechanism.

## Topics

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

var BLAS_THREADING_MAX_OPTIONS: BLAS_THREADING

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the threading model

struct BLAS

An enumeration that acts as a namespace for Swift overlays to BLAS.

func BLASSetThreading(BLAS_THREADING) -> Int32

Sets the BLAS and LAPACK threading model.

func BLASGetThreading() -> BLAS_THREADING

Returns the current BLAS and LAPACK threading model.

