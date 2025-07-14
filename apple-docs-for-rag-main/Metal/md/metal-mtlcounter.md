

- Metal
-  MTLCounter 

Protocol

# MTLCounter

An individual counter a GPU device lists within one of its counter sets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLCounter : NSObjectProtocol
```

## Overview

You can determine which counters a GPU supports within a counter set (see MTLCounterSet) by checking the elements of its counters property. A counter’s name property typically matches one of the common counter set names that MTLCommonCounter defines. For more information, see Confirming which Counters and Counter Sets a GPU Supports.

## Topics

### Identifying a Counter

var name: String

The name of a GPU’s counter instance.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Counters and Counter Sets

Confirming which Counters and Counter Sets a GPU Supports

Check whether a GPU produces the runtime performance data you want to sample.

protocol MTLCounterSet

A collection of individual counters a GPU device supports for a counter set.

struct MTLCommonCounterSet

The name of a specific counter set that a GPU device can support.

struct MTLCommonCounter

The name of a specific counter that can appear in a GPU device’s counter sets.

