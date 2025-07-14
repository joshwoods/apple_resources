

- Latent Semantic Mapping
- LSMResult
-  Result Flags 

API Collection

# Result Flags

Options for creating a result.

## Overview

Specify these options for LSMResultCreate(_:_:_:_:_:).

## Topics

### Constants

var kLSMResultBestWords: Int

Finds the words, rather than categories, that best match.

## See Also

### Creating a Result

func LSMResultCreate(CFAllocator?, LSMMap, LSMText, CFIndex, CFOptionFlags) -> Unmanaged&lt;LSMResult>

Returns the categories or words that best match when a text is mapped into a map, in decreasing order of likelihood.

