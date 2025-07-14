

- Distributed
- DistributedActorSystem
-  resignID(\_:) 

Instance Method

# resignID(\_:)

Called during when a distributed actor is deinitialized, or fails to initialize completely (e.g. by throwing out of an `init` that did not completely initialize all of the actors stored properties yet).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func resignID(_ id: Self.ActorID)
```

**Required**

## Parameters 

`id`  

The id of an actor managed by this system that has begun its `deinit`.

## Discussion

This method is guaranteed to be called at-most-once for a given id (assuming IDs are unique, and not re-cycled by the system), i.e. if it is called during a failure to initialize completely, the call from the actor’s deinitializer will not happen (as under these circumstances, `deinit` will be run).

If `resignID` gets called with some unknown ID, it should crash immediately as it signifies some very unexpected use of the system.

