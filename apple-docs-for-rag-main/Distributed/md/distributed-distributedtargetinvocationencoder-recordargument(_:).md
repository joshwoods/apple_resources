

- Distributed
- DistributedTargetInvocationEncoder
-  recordArgument(\_:) 

Instance Method

# recordArgument(\_:)

Record an argument of `Argument` type. This will be invoked for every argument of the target, in declaration order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func recordArgument(_ argument: RemoteCallArgument) throws
```

**Required**

### Serialization Requirement

Implementations of this method must ensure that the `Value` type parameter conforms to the types’ `SerializationRequirement`.

