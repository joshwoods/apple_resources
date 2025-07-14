

- Foundation
- FileManager
-  FileManager.URLRelationship 

Enumeration

# FileManager.URLRelationship

Constants indicating the relationship between a directory and an item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum URLRelationship
```

## Topics

### URL Relationships

case contains

The directory contains the specified item.

case same

The directory and the item are the same. This relationship occurs when the value of the fileResourceIdentifierKey is the same for the directory and item.

case other

The directory does not contain the item and is not the same as the item.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Relationship Between Items

func getRelationship(UnsafeMutablePointer&lt;FileManager.URLRelationship>, ofDirectoryAt: URL, toItemAt: URL) throws

Determines the type of relationship that exists between a directory and an item.

func getRelationship(UnsafeMutablePointer&lt;FileManager.URLRelationship>, of: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, toItemAt: URL) throws

Determines the type of relationship that exists between a system directory and the specified item.

