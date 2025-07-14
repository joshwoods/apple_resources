

- Combine
- TopLevelDecoder
-  decode(\_:from:) 

Instance Method

# decode(\_:from:)

Decodes an instance of the indicated type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func decode(
    _ type: T.Type,
    from: Self.Input
) throws -> T where T : Decodable
```

**Required**

