

- SwiftUI
- NavigationPath
-  codable 

Instance Property

# codable

A value that describes the contents of this path in a serializable format.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var codable: NavigationPath.CodableRepresentation? { get }
```

## Discussion

This value is `nil` if any of the type-erased elements of the path don’t conform to the Codable protocol.

## See Also

### Encoding a path

struct CodableRepresentation

A serializable representation of a navigation path.

