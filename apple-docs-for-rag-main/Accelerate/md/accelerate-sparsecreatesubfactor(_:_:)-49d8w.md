

- Accelerate
-  SparseCreateSubfactor(\_:\_:) 

Function

# SparseCreateSubfactor(\_:\_:)

Returns an opaque object that represents a subfactor of a factorization of a matrix of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseCreateSubfactor(
    _ subfactor: SparseSubfactor_t,
    _ Factor: SparseOpaqueFactorization_Double
) -> SparseOpaqueSubfactor_Double
```

## Parameters 

`subfactor`  

Defines which subfactor to extract.

`Factor`  

The factorization to extract the subfactor from.

## Return Value

A `SparseOpaqueSubfactor_Double` structure that represents the subfactor. You must free the resource through a call to SparseCleanup(_:) after you finish with the object.

## See Also

### Subfactor Extraction

struct SparseSubfactor_t

Constants that define the subfactor of a factorization.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

func SparseCreateSubfactor(SparseSubfactor_t, SparseOpaqueFactorization_Float) -> SparseOpaqueSubfactor_Float

Returns an opaque object that represents a subfactor of a factorization of a matrix of single-precision values.

struct SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

