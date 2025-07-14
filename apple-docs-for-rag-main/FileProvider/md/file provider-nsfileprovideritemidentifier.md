

- File Provider
-  NSFileProviderItemIdentifier 

Structure

# NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

iOS 8.0+iPadOS 8.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderItemIdentifier
```

## Topics

### Constants

static let rootContainer: NSFileProviderItemIdentifier

The persistent identifier for the root directory of the file provider’s shared file hierarchy.

static let workingSet: NSFileProviderItemIdentifier

The persistent identifier representing the working set of documents and directories.

static let trashContainer: NSFileProviderItemIdentifier

The persistent identifier for the parent of all trashed items.

### Initializers

init(String)

Returns a newly instantiated persistent identifier.

init(rawValue: String)

Returns a newly instantiated persistent identifier.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Provided items

typealias NSFileProviderItem

An item the File Provider extension manages.

protocol NSFileProviderItemProtocol

A protocol that defines the properties of an item managed by the File Provider extension.

struct NSFileProviderItemCapabilities

An item’s capabilities, which define the actions that the user can perform in the document browser.

struct NSFileProviderTypeAndCreator

A structure that contains the file type and file creator codes for an item.

