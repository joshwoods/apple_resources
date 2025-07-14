

- System
- FilePath
-  FilePath.ComponentView 

Structure

# FilePath.ComponentView

A bidirectional, range replaceable collection of the non-root components that make up a file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ComponentView
```

## Overview

ComponentView provides access to standard `BidirectionalCollection` algorithms for accessing components from the front or back, as well as standard `RangeReplaceableCollection` algorithms for modifying the file path using component or range of components granularity.

Example:

```
var path: FilePath = "/./home/./username/scripts/./tree"
let scriptIdx = path.components.lastIndex(of: "scripts")!
path.components.insert("bin", at: scriptIdx)
// path is "/./home/./username/bin/scripts/./tree"

path.components.removeAll { $0.kind == .currentDirectory }
// path is "/home/username/bin/scripts/tree"
```

## Topics

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RangeReplaceableCollection
- Sendable
- Sequence

