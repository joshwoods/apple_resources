

- File Provider
-  NSFileProviderKnownFolders 

Structure

# NSFileProviderKnownFolders

Constants that identify known folders.

macOS 15.0+

``` source
struct NSFileProviderKnownFolders
```

## Topics

### Identifying known folders

static var desktop: NSFileProviderKnownFolders

static var documents: NSFileProviderKnownFolders

### Creating a known-folder identifier

init(rawValue: UInt)

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

### Syncing Desktop and Documents folders

var replicatedKnownFolders: NSFileProviderKnownFolders

A list of known folders that the domain currently replicates.

var supportedKnownFolders: NSFileProviderKnownFolders

A list of known folders that the domain can replicate.

