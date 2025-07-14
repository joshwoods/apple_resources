

- File Provider
-  NSFileProviderMaterializationFlags 

Structure

# NSFileProviderMaterializationFlags

Flags that provides additional information about the provided content.

macOS 12.3+

``` source
struct NSFileProviderMaterializationFlags
```

## Topics

### Accessing Flags

static var knownSparseRanges: NSFileProviderMaterializationFlags

A flag indicating that the system should consider the file fully materialized, even if it’s a sparse file.

### Creating Flags

init(rawValue: UInt)

Creates a new materialization flag.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Fetching Ranges from a File

func fetchPartialContents(for: NSFileProviderItemIdentifier, version: NSFileProviderItemVersion, request: NSFileProviderRequest, minimalRange: NSRange, aligningTo: Int, options: NSFileProviderFetchContentsOptions, completionHandler: (URL?, NSFileProviderItem?, NSRange, NSFileProviderMaterializationFlags, (any Error)?) -> Void) -> Progress

Tells the file provider to download the requested item from remote storage.

**Required**

struct NSFileProviderFetchContentsOptions

Options for fetching a range of data from a file.

