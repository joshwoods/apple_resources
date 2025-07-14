

- Distributed
- DistributedTargetInvocationResultHandler
-  onThrow(error:) 

Instance Method

# onThrow(error:)

Invoked when the distributed target execution of a target has thrown an error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func onThrow(error: Err) async throws where Err : Error
```

**Required**

## Discussion

It is not guaranteed that the error conform to the SerializationRequirement; This guarantee is only given to return values (and offered by `onReturn`).

