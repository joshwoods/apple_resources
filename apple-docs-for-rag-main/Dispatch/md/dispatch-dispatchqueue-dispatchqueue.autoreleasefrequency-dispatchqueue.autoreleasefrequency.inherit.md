

- Dispatch
- DispatchQueue
- DispatchQueue.AutoreleaseFrequency
-  DispatchQueue.AutoreleaseFrequency.inherit 

Case

# DispatchQueue.AutoreleaseFrequency.inherit

The queue inherits its autorelease frequency from its target queue.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case inherit
```

## Discussion

This option is the default behavior for queues you create.

## See Also

### Autorelease Frequencies

case workItem

The queue configures an autorelease pool before the execution of a block, and releases the objects in that pool after the block finishes executing.

case never

The queue does not set up an autorelease pool around executed blocks.

