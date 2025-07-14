

- Create ML Components
- EstimatorDecoder
-  decodeOptimizer(\_:) 

Instance Method

# decodeOptimizer(\_:)

Decodes an optimizer value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func decodeOptimizer(_ value: T.Type) throws -> T where T : Decodable
```

**Required**

## Discussion

Decoding an optimizer lets you resume fitting.

## See Also

### Decoding values

func decode&lt;T>(T.Type) throws -> T

Decodes a value.

**Required**

