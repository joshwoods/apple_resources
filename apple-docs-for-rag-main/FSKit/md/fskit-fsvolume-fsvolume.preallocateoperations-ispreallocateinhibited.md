

- FSKit
- FSVolume
- FSVolume.PreallocateOperations
-  isPreallocateInhibited 

Instance Property

# isPreallocateInhibited

A Boolean value that instructs FSKit not to call this protocol’s methods, even if the volume conforms to it.

macOS 15.4+

``` source
optional var isPreallocateInhibited: Bool { get set }
```

## Discussion

FSKit reads this value after the file system replies to the `loadResource` message. Changing the returned value during the runtime of the volume has no effect.

