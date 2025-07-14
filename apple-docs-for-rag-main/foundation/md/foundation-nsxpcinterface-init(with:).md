

- Foundation
- NSXPCInterface
-  init(with:) 

Initializer

# init(with:)

Returns an NSXPCInterface instance for a given protocol.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(with protocol: Protocol)
```

## Discussion

Most interfaces do not need any further configuration. Interfaces with collection classes or additional proxy objects should be configured using the other methods in this class.

