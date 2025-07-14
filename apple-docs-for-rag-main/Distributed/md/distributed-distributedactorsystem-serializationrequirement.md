

- Distributed
- DistributedActorSystem
-  SerializationRequirement 

Associated Type

# SerializationRequirement

The serialization requirement that will be applied to all distributed targets used with this system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
associatedtype SerializationRequirement where Self.SerializationRequirement == Self.InvocationDecoder.SerializationRequirement
```

**Required**

