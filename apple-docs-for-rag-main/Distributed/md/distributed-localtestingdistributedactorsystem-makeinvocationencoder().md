

- Distributed
- LocalTestingDistributedActorSystem
-  makeInvocationEncoder() 

Instance Method

# makeInvocationEncoder()

Invoked by the Swift runtime when a distributed remote call is about to be made.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final func makeInvocationEncoder() -> LocalTestingDistributedActorSystem.InvocationEncoder
```

## Discussion

The returned `DistributedTargetInvocation` will be populated with all arguments, generic substitutions, and specific error and return types that are associated with this specific invocation.

