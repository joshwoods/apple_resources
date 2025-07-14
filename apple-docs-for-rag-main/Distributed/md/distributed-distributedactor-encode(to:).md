

- Distributed
- DistributedActor
-  encode(to:) 

Instance Method

# encode(to:)

Encodes the `actor.id` as a single value into the passed `encoder`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func encode(to encoder: any Encoder) throws
```

Available when `ID` conforms to `Encodable`.

