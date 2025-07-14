

- Core Media I/O
- CMIOExtensionScheduledOutput
-  init(sequenceNumber:hostTimeInNanoseconds:) 

Initializer

# init(sequenceNumber:hostTimeInNanoseconds:)

Creates a scheduled output object.

Mac Catalyst 15.4+macOS 12.3+

``` source
init(
    sequenceNumber: UInt64,
    hostTimeInNanoseconds: UInt64
)
```

## Parameters 

`sequenceNumber`  

The buffer sequence number that was output.

`hostTimeInNanoseconds`  

The host time in nanoseconds when the buffer was output.

