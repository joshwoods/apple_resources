

- Distributed
- DistributedActorSystem
-  ActorID 

Associated Type

# ActorID

The type ID that will be assigned to any distributed actor managed by this actor system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
associatedtype ActorID : Hashable, Sendable
```

**Required**

### A note on Codable IDs

If this type is `Codable`, then any `distributed actor` using this `ActorID` as its `DistributedActor/ID` will gain a synthesized `Codable` conformance which is implemented by encoding the `ID`. The decoding counter part of the `Codable` conformance is implemented by decoding the `ID` and passing it to the resolve(id:using:) method.

