

- Dispatch
- DispatchQueue
- DispatchQueue.AutoreleaseFrequency
-  DispatchQueue.AutoreleaseFrequency.workItem 

Case

# DispatchQueue.AutoreleaseFrequency.workItem

The queue configures an autorelease pool before the execution of a block, and releases the objects in that pool after the block finishes executing.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
case workItem
```

## See Also

### Autorelease Frequencies

case inherit

The queue inherits its autorelease frequency from its target queue.

case never

The queue does not set up an autorelease pool around executed blocks.

