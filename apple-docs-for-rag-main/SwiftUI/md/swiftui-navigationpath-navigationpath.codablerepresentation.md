

- SwiftUI
- NavigationPath
-  NavigationPath.CodableRepresentation 

Structure

# NavigationPath.CodableRepresentation

A serializable representation of a navigation path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct CodableRepresentation
```

## Overview

When a navigation path contains elements the conform to the Codable protocol, you can use the path’s `CodableRepresentation` to convert the path to an external representation and to convert an external representation back into a navigation path.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable

## See Also

### Encoding a path

var codable: NavigationPath.CodableRepresentation?

A value that describes the contents of this path in a serializable format.

