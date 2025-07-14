

- Distributed
- LocalTestingInvocationEncoder
-  recordReturnType(\_:) 

Instance Method

# recordReturnType(\_:)

Record the return type of the distributed method. This method will not be invoked if the target is returning `Void`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func recordReturnType(_ type: R.Type) throws where R : Decodable, R : Encodable
```

### Serialization Requirement

Implementations of this method must ensure that the `R` type parameter conforms to the types’ `SerializationRequirement`.

