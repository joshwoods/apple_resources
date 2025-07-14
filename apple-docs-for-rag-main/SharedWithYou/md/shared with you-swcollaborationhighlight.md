

- Shared With You
-  SWCollaborationHighlight 

Class

# SWCollaborationHighlight

A highlight object that represents an active collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationHighlight
```

## Mentioned in 

Adding shared content collaboration to your app

Adding custom collaboration to your app

## Topics

### Accessing collaboration attributes

var collaborationIdentifier: String

A unique identifier that the app hosting the collaboration provides.

var contentType: UTType

The UTI type for this collaboration highlight.

var creationDate: Date

The date the system creates this file.

var title: String?

The title of the collaboration highlight.

## Relationships

### Inherits From

- SWHighlight

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Collaboration attributes

class SWCollaborationMetadata

A model object for conveying data during a collaboration.

struct SWCollaborationIdentifier

A unique identifier for a collaboration.

struct SWLocalCollaborationIdentifier

A local identifier for a collaboration.

let SWCollaborationMetadataTypeIdentifier: String

A string constant for the metadata type identifier.

