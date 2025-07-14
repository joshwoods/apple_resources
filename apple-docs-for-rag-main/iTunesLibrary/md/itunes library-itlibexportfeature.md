

- iTunes Library
-  ITLibExportFeature 

Enumeration

# ITLibExportFeature

These constants describe the features that an iTunes library supports.

Mac Catalyst 14.0+macOS 10.13+

``` source
enum ITLibExportFeature
```

## Topics

### Export Features

case none

The iTunes library doesn’t support any export features.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

var features: ITLibExportFeature

A bitwise OR combination of the features of this library.

Deprecated

var musicFolderLocation: URL?

The location of the iTunes music folder.

Deprecated

