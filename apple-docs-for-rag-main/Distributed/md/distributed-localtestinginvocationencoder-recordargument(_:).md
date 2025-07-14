

- Distributed
- LocalTestingInvocationEncoder
-  recordArgument(\_:) 

Instance Method

# recordArgument(\_:)

Record an argument of `Argument` type. This will be invoked for every argument of the target, in declaration order.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func recordArgument(_ argument: RemoteCallArgument) throws where Value : Decodable, Value : Encodable
```

### Serialization Requirement

Implementations of this method must ensure that the `Value` type parameter conforms to the types’ `SerializationRequirement`.

