

- Metal
-  MTLCommonCounterSet 

Structure

# MTLCommonCounterSet

The name of a specific counter set that a GPU device can support.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCommonCounterSet
```

## Mentioned in 

Confirming which Counters and Counter Sets a GPU Supports

## Overview

This type defines the constants that let a GPU device declare which counter sets it supports.

Important

Some GPUs may only support some of the counters within a counter set.

For more information, see Confirming which Counters and Counter Sets a GPU Supports.

## Topics

### Common Counter Set Names

static let timestamp: MTLCommonCounterSet

The common name for the counter set that contains the timestamp counter.

static let stageUtilization: MTLCommonCounterSet

The common name for the counter set that contains hardware utilization measurements from various render stages.

static let statistic: MTLCommonCounterSet

The common name for the counter set that contains GPU workload statistics.

### Swift Support

init(rawValue: String)

Creates a common counter set name from a raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Counters and Counter Sets

Confirming which Counters and Counter Sets a GPU Supports

Check whether a GPU produces the runtime performance data you want to sample.

protocol MTLCounterSet

A collection of individual counters a GPU device supports for a counter set.

protocol MTLCounter

An individual counter a GPU device lists within one of its counter sets.

struct MTLCommonCounter

The name of a specific counter that can appear in a GPU device’s counter sets.

