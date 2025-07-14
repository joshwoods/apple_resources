

- Distributed
- LocalTestingInvocationResultHandler
-  onReturn(value:) 

Instance Method

# onReturn(value:)

Invoked when the distributed target execution returns successfully. The `value` is the return value of the executed distributed invocation target.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func onReturn(value: Success) async throws where Success : Decodable, Success : Encodable
```

### Serialization Requirement

Implementations of this method must ensure that the `Success` type parameter conforms to the types’ `SerializationRequirement`.

