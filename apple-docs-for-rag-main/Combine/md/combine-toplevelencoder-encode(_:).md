

- Combine
- TopLevelEncoder
-  encode(\_:) 

Instance Method

# encode(\_:)

Encodes an instance of the indicated type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func encode(_ value: T) throws -> Self.Output where T : Encodable
```

**Required**

## Parameters 

`value`  

The instance to encode.

