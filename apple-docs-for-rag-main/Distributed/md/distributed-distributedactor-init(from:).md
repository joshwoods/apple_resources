

- Distributed
- DistributedActor
-  init(from:) 

Initializer

# init(from:)

Initializes an instance of this distributed actor by decoding its id, and passing it to the DistributedActorSystem obtained from `decoder.userInfo[actorSystemKey]`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
init(from decoder: any Decoder) throws
```

Available when `ID` conforms to `Decodable`.

## Parameters 

`decoder`  

Used to decode the `ID` of this distributed actor.

## Requires: The decoder must have the ``CodingUserInfoKey/actorSystemKey`` set to

the ActorSystem that this actor expects, as it will be used to call resolve(id:using:) on, in order to obtain the instance this initializer should return.

Throws

If the actor system value in `decoder.userInfo` is missing or mistyped; the `ID` fails to decode from the passed `decoder`;

