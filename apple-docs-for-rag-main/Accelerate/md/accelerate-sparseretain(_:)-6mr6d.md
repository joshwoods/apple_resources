

- Accelerate
-  SparseRetain(\_:) 

Function

# SparseRetain(\_:)

Increases the reference count on a single-precision subfactor object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseRetain(_ Subfactor: SparseOpaqueSubfactor_Float) -> SparseOpaqueSubfactor_Float
```

## Parameters 

`Subfactor`  

The subfactor object to increase the reference count upon.

## Return Value

The supplied numeric subfactor object.

## See Also

### Resource Retention

func SparseRetain(SparseOpaqueSymbolicFactorization) -> SparseOpaqueSymbolicFactorization

Increases the reference count on a symbolic factorization object.

func SparseRetain(SparseOpaqueFactorization_Double) -> SparseOpaqueFactorization_Double

Increases the reference count on a double-precision numeric factorization object.

func SparseRetain(SparseOpaqueFactorization_Float) -> SparseOpaqueFactorization_Float

Increases the reference count on a single-precision numeric factorization object.

func SparseRetain(SparseOpaqueSubfactor_Double) -> SparseOpaqueSubfactor_Double

Increases the reference count on a double-precision subfactor object.

