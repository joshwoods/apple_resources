

- Core Transferable
-  TransferRepresentationVisibility 

Structure

# TransferRepresentationVisibility

The visibility levels that specify the kinds of apps and processes that can see an item in transit.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct TransferRepresentationVisibility
```

## Topics

### Specifying transfer visibility

static let all: TransferRepresentationVisibility

The visibility level that specifies that any app or process can access the item.

static let team: TransferRepresentationVisibility

The visibility level that specifies that the item is visible only to apps created by the current app’s development team.

static let group: TransferRepresentationVisibility

The visibility level that specifies that the item is visible only to macOS apps in the same App Group.

static let ownProcess: TransferRepresentationVisibility

The visibility level that specifies that the item is visible only within the app that’s the source of the item.

### Operators

static func == (TransferRepresentationVisibility, TransferRepresentationVisibility) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Transfer customization

struct ProxyRepresentation

A transfer representation that uses another type’s transfer representation as its own.

