

- Latent Semantic Mapping
-  LSMResult 

Class

# LSMResult

A result of a lookup in a map.

Mac CatalystmacOS

``` source
class LSMResult
```

## Overview

An LSMResult is an immutable, opaque Core Foundation type that represents the result of a lookup.

## Topics

### Creating a Result

func LSMResultCreate(CFAllocator?, LSMMap, LSMText, CFIndex, CFOptionFlags) -> Unmanaged&lt;LSMResult>

Returns the categories or words that best match when a text is mapped into a map, in decreasing order of likelihood.

Result Flags

Options for creating a result.

### Querying Result Information

func LSMResultGetCount(LSMResult) -> CFIndex

Returns the number of results.

func LSMResultGetCategory(LSMResult, CFIndex) -> LSMCategory

Returns the category of the specified result.

func LSMResultGetScore(LSMResult, CFIndex) -> Float

Returns the likelihood of the specified result.

### Getting a Result

func LSMResultCopyToken(LSMResult, CFIndex) -> Unmanaged&lt;CFData>?

Returns the token for the n-th best (zero-based) result.

func LSMResultCopyTokenCluster(LSMResult, CFIndex) -> Unmanaged&lt;CFArray>?

Returns the cluster of tokens for the n-th best (zero-based) result.

func LSMResultCopyWord(LSMResult, CFIndex) -> Unmanaged&lt;CFString>?

Returns the word for the n-th best (zero-based) result.

func LSMResultCopyWordCluster(LSMResult, CFIndex) -> Unmanaged&lt;CFArray>?

Returns the cluster of words for the n-th best (zero-based) result.

### Getting the Type Identifier

func LSMResultGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for Latent Semantic Mapping results.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Text Classification

class LSMMap

A map between a set of categories and related text.

class LSMText

An input text.

