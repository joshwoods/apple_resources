

- Core Services
- Apple Events
-  AERemoteProcessResolverRef 

Type Alias

# AERemoteProcessResolverRef

An opaque reference to an object that encapsulates the mechanism for obtaining a list of processes running on a remote machine.

Mac Catalyst 13.0+macOS 10.3+

``` source
typealias AERemoteProcessResolverRef = OpaquePointer
```

## Discussion

You create an instance of `AERemoteProcessResolverRef` by calling AECreateRemoteProcessResolver(_:_:), and you must disposed of it by calling AEDisposeRemoteProcessResolver(_:). An instance of this type is not a `CFType` (the base type used by all Core Foundation derived opaque types).

