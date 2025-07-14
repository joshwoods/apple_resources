

- Distributed
- DistributedActor
-  SerializationRequirement 

Associated Type

# SerializationRequirement

The serialization requirement to apply to all distributed declarations inside the actor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
associatedtype SerializationRequirement where Self.SerializationRequirement == Self.ActorSystem.SerializationRequirement
```

**Required**

