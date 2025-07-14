

- Metal
-  MTLCounterResultTimestamp 

Structure

# MTLCounterResultTimestamp

The data structure for storing the data you resolve from a timestamp counter set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCounterResultTimestamp
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Overview

For steps that explain how to resolve data from a counter set, such as timestamp, see Converting a GPU’s Counter Data into a Readable Format.

## Topics

### Timestamp Values

var timestamp: UInt64

A timestamp value from a GPU at a particular point in time during an operation, typically at the beginning or ending of a render stage.

### Swift Support

init()

Creates a default timestamp result.

init(timestamp: UInt64)

Creates a timestamp result from a value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Counter Sample Data Output

Converting a GPU’s Counter Data into a Readable Format

Inspect and use the data within a GPU’s counter sample buffer by resolving it into a standard format.

struct MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

struct MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

var MTLCounterErrorValue: UInt64

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

