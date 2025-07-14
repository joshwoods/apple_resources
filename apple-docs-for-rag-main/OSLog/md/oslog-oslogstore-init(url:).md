

- OSLog
- OSLogStore
-  init(url:) 

Initializer

# init(url:)

Creates a log store based on a log archive.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(url: URL) throws
```

## See Also

### Creating Log Stores

class func local() throws -> Self

Creates a log store representing the Mac’s local store.

