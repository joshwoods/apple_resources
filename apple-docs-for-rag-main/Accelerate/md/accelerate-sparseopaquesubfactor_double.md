

- Accelerate
-  SparseOpaqueSubfactor_Double 

Structure

# SparseOpaqueSubfactor_Double

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseOpaqueSubfactor_Double
```

## Overview

Attributes of subfactor. Notably transpose indicates whether it should be considered as the transpose of its underlying contents (e.g. should it count as L or L^T if .contents=SparseSubfactorL).

Subfactor this represents, e.g. L or Q.

Underlying factorization this subfactor is part of.

The size of the workspace, in bytes, required to perform SparseMultiply() or SparseSolve() with this subfactor is given by the expression: workspaceRequiredStatic + nrhs\*workspaceRequiredPerRhs where nrhs is the number of right-hand side vectors.

The size of the workspace, in bytes, required to perform SparseMultiply() or SparseSolve() with this subfactor is given by the expression: workspaceRequiredStatic + nrhs\*workspaceRequiredPerRhs where nrhs is the number of right-hand side vectors.

## Topics

### Initializers

init()

init(attributes: SparseAttributes_t, contents: SparseSubfactor_t, factor: SparseOpaqueFactorization_Double, workspaceRequiredStatic: Int, workspaceRequiredPerRHS: Int)

### Instance Properties

var attributes: SparseAttributes_t

var contents: SparseSubfactor_t

var factor: SparseOpaqueFactorization_Double

var workspaceRequiredPerRHS: Int

var workspaceRequiredStatic: Int

## See Also

### Structures

struct SparseOpaqueSubfactor_Float

