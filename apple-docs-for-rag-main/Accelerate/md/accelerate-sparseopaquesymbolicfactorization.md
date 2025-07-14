

- Accelerate
-  SparseOpaqueSymbolicFactorization 

Structure

# SparseOpaqueSymbolicFactorization

A semi-opaque type that represents symbolic matrix factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseOpaqueSymbolicFactorization
```

## Overview

Represents a symbolic matrix factorization (that is, the pattern of the factors without the values). A single symbolic factorization may be the basis for multiple numerical factorizations of matrices with the same pattern but different nonzero values.

Use the SparseCleanup(_:) function to free resources that these objects hold. The system reference-counts the internal factorize pointer, so it’s safe to destroy this object even if numeric factorizations exist that still depend on it.

## Topics

### Creating an Opaque Symbolic Factorization

init()

init(status: SparseStatus_t, rowCount: Int32, columnCount: Int32, attributes: SparseAttributes_t, blockSize: UInt8, type: SparseFactorization_t, factorization: UnsafeMutableRawPointer?, workspaceSize_Float: Int, workspaceSize_Double: Int, factorSize_Float: Int, factorSize_Double: Int)

Creates an opaque symbolic factorization.

### Instance Properties

var status: SparseStatus_t

The status of the factorization.

struct SparseStatus_t

Constants that describe the status of a factorization.

var type: SparseFactorization_t

The factorization type.

var factorization: UnsafeMutableRawPointer?

A pointer to a private internal representation of the symbolic factor.

struct SparseFactorization_t

Constants that define the factorization type.

### Inspecting a Factorization’s Structure

var attributes: SparseAttributes_t

The attributes of the factorization.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var blockSize: UInt8

The block size.

var columnCount: Int32

The number of columns.

var rowCount: Int32

The number of rows.

var workspaceSize_Double: Int

Size, in bytes, of workspace required to perform numerical factorization in doubles.

var workspaceSize_Float: Int

Size, in bytes, of workspace required to perform numerical factorization in floats.

var factorSize_Double: Int

Minimum size, in bytes, required to store numerical factors in doubles.

var factorSize_Float: Int

Minimum size, in bytes, required to store numerical factors in float.

## See Also

### Supporting Types

struct SparseFactorization_t

Constants that define the factorization type.

struct SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

