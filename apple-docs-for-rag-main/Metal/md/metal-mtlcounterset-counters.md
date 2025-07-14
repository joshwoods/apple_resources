

- Metal
- MTLCounterSet
-  counters 

Instance Property

# counters

An array of the counter instances a GPU device supports.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var counters: [any MTLCounter] { get }
```

**Required**

## Mentioned in 

Confirming which Counters and Counter Sets a GPU Supports

## Discussion

Check whether a GPU device supports a specific counter by comparing its common name (see MTLCommonCounter) with each element in the property’s array.

Important

Some GPUs may only support some of the counters within a counter set.

For more information, see Confirming which Counters and Counter Sets a GPU Supports.

