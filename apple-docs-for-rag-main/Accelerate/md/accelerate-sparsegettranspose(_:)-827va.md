

- Accelerate
-  SparseGetTranspose(\_:) 

Function

# SparseGetTranspose(\_:)

Returns a transposed copy of the specified single-precision subfactor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseGetTranspose(_ Subfactor: SparseOpaqueSubfactor_Float) -> SparseOpaqueSubfactor_Float
```

## Parameters 

`Subfactor`  

The subfactor to transpose.

## Return Value

An object equivalent to the transpose of the one you provide. Because this is a reference-counted subfactor, the system must free it through a call to SparseCleanup(_:) when it no longer needs it.

## See Also

### Subfactor Transpose Functions

func SparseGetTranspose(SparseOpaqueSubfactor_Double) -> SparseOpaqueSubfactor_Double

Returns a transposed copy of the specified double-precision subfactor.

