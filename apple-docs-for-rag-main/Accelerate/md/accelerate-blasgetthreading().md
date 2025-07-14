

- Accelerate
-  BLASGetThreading() 

Function

# BLASGetThreading()

Returns the current BLAS and LAPACK threading model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BLASGetThreading() -> BLAS_THREADING
```

## Return Value

A constant that represents the current BLAS and LAPACK threading model.

## See Also

### Specifying the threading model

struct BLAS

An enumeration that acts as a namespace for Swift overlays to BLAS.

func BLASSetThreading(BLAS_THREADING) -> Int32

Sets the BLAS and LAPACK threading model.

struct BLAS_THREADING

Constants that describe the BLAS and LAPACK threading model.

