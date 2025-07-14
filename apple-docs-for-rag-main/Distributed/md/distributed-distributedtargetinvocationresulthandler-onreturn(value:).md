

- Distributed
- DistributedTargetInvocationResultHandler
-  onReturn(value:) 

Instance Method

# onReturn(value:)

Invoked when the distributed target execution returns successfully. The `value` is the return value of the executed distributed invocation target.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func onReturn(value: Success) async throws
```

**Required**

### Serialization Requirement

Implementations of this method must ensure that the `Success` type parameter conforms to the types’ `SerializationRequirement`.

