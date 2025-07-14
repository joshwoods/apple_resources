

- Metal
-  MTLCounterSet 

Protocol

# MTLCounterSet

A collection of individual counters a GPU device supports for a counter set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLCounterSet : NSObjectProtocol
```

## Overview

You can determine which counter sets a GPU supports by checking an MTLDevice instance’s counterSets property. A counter set’s name property typically matches one of the common counter set names that MTLCommonCounterSet defines. Check whether a GPU device supports a specific counter by comparing elements of the counters property with a counter’s common name that MTLCommonCounter defines.

Important

Some GPUs may only support some of the counters within a counter set.

For more information, see Confirming which Counters and Counter Sets a GPU Supports.

## Topics

### Identifying a Counter Set

var name: String

The name of the GPU’s counter set instance.

**Required**

### Checking Which Counters a GPU Supports

var counters: [any MTLCounter]

An array of the counter instances a GPU device supports.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Counters and Counter Sets

Confirming which Counters and Counter Sets a GPU Supports

Check whether a GPU produces the runtime performance data you want to sample.

struct MTLCommonCounterSet

The name of a specific counter set that a GPU device can support.

protocol MTLCounter

An individual counter a GPU device lists within one of its counter sets.

struct MTLCommonCounter

The name of a specific counter that can appear in a GPU device’s counter sets.

