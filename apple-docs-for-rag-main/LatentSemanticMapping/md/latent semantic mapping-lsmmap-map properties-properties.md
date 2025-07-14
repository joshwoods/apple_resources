

- Latent Semantic Mapping
- LSMMap
-  Map Properties 

API Collection

# Map Properties

Special properties that determine a map’s behavior.

## Overview

Latent Semantic Mapping interprets the following keys. All other keys starting with `LSM` are reserved.

## Topics

### Properties

var kLSMAlgorithmKey: String

A key that specifies which algorithm to use.

var kLSMAlgorithmDense: String

A value that specifies to perform a singular value decomposition (SVD) on a dense matrix.

var kLSMAlgorithmSparse: String

A value that specifies to perform a singular value decomposition (SVD) on a sparse matrix.

var kLSMPrecisionKey: String

A key that specifies the precision to use.

var kLSMPrecisionFloat: String

A value that specifies to use float arithmetic.

var kLSMPrecisionDouble: String

A value that specifies to use double arithmetic.

var kLSMDimensionKey: String

A key that specifies the number of singular values to compute.

var kLSMIterationsKey: String

A key that specifies the number of iterations to compute.

var kLSMSweepAgeKey: String

A key that specifies the number of days between sweeping generations.

var kLSMSweepCutoffKey: String

A key that specifies the minimum count to keep entry.

## See Also

### Managing a Map’s Properties

func LSMMapSetProperties(LSMMap, CFDictionary)

Sets a dictionary of properties for the map.

func LSMMapGetProperties(LSMMap) -> Unmanaged&lt;CFDictionary>

Gets a dictionary of properties for the map.

