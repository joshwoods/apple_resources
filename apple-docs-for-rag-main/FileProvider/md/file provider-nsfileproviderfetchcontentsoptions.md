

- File Provider
-  NSFileProviderFetchContentsOptions 

Structure

# NSFileProviderFetchContentsOptions

Options for fetching a range of data from a file.

macOS 12.3+

``` source
struct NSFileProviderFetchContentsOptions
```

## Topics

### Accessing Options

static var strictVersioning: NSFileProviderFetchContentsOptions

An option that indicates the system requires an exact match of the requested item’s version.

### Creating Options

init(rawValue: UInt)

Creates an option instance from the raw value.

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

struct NSFileProviderMaterializationFlags

Flags that provides additional information about the provided content.

