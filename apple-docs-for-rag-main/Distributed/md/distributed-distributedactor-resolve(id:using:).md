

- Distributed
- DistributedActor
-  resolve(id:using:) 

Type Method

# resolve(id:using:)

Resolves the passed in `id` against the `system`, returning either a local or remote actor reference.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func resolve(
    id: Self.ID,
    using system: Self.ActorSystem
) throws -> Self
```

**Required**

## Parameters 

`id`  

Identity uniquely identifying a, potentially remote, actor in the system

`system`  

`system` which should be used to resolve the `identity`, and be associated with the returned actor

## Discussion

The system will be asked to `resolve` the identity and return either a local instance or request a proxy to be created for this identity.

A remote distributed actor reference will forward all invocations through the system, allowing it to take over the remote messaging with the remote actor instance.

Postcondition

Upon successful return, the returned actor’s id and actorSystem properties will be equal to the values passed as parameters to this method.

