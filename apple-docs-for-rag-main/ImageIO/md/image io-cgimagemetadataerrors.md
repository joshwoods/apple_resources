

- Image I/O
-  CGImageMetadataErrors 

Enumeration

# CGImageMetadataErrors

Constants for errors that occur when getting or setting metadata information.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CGImageMetadataErrors
```

## Topics

### Error Codes

case unknown

An error that indicates an unknown condition occurred.

case unsupportedFormat

An error that indicates the metadata was in an unsupported format.

case badArgument

An error that indicates a parameter was malformed or contained invalid data.

case conflictingArguments

An error that indicates an attempt to save conflicting metadata values.

case prefixConflict

An error that indicates an attempt to register a namespace with a prefix that is different than the namespace’s existing prefix.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### XMP Metadata

class CGImageMetadata

An immutable object that contains the XMP metadata associated with an image.

class CGMutableImageMetadata

An opaque type for adding or modifying image metadata.

class CGImageMetadataTag

An immutable type that contains information about a single piece of image metadata.

XMP Namespaces and Prefixes

Discover the public namespaces and prefixes that exist in XMP metadata tags.

let kCFErrorDomainCGImageMetadata: CFString

The domain for metadata-related errors that originate in the Image I/O framework.

