

- Distributed
- DistributedActorSystem
-  InvocationDecoder 

Associated Type

# InvocationDecoder

Type of DistributedTargetInvocationDecoder that should be used when decoding invocations during executeDistributedTarget(on:target:invocationDecoder:handler:) calls.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
associatedtype InvocationDecoder : DistributedTargetInvocationDecoder where Self.InvocationDecoder.SerializationRequirement == Self.InvocationEncoder.SerializationRequirement
```

**Required**

