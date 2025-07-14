

- SwiftData
- PersistentIdentifier
-  identifier(for:entityName:primaryKey:) 

Type Method

# identifier(for:entityName:primaryKey:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 10.0+Swift 5.9+

``` source
static func identifier(
    for storeIdentifier: String,
    entityName: String,
    primaryKey: T
) throws -> PersistentIdentifier where T : Comparable, T : CustomStringConvertible, T : Decodable, T : Encodable, T : Hashable
```

