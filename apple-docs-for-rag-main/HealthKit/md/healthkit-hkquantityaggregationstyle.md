

- HealthKit
-  HKQuantityAggregationStyle 

Enumeration

# HKQuantityAggregationStyle

Constant values that describe how quantities can be aggregated over time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKQuantityAggregationStyle
```

## Overview

A quantity type’s aggregation style determines the type of statistics queries that you can perform. Discrete types support average, minimum, and maximum queries. Cumulative types support only sum queries. For more information, see HKStatisticsQuery.

## Topics

### Aggregation Styles

case cumulative

Cumulative samples that can be summed over time.

case discreteArithmetic

Discrete samples that can be averaged over time using an arithmetic mean.

case discreteTemporallyWeighted

Discrete samples that can be averaged over a time interval using a temporally weighted integration function.

case discreteEquivalentContinuousLevel

Discrete samples that can be combined over a time interval by computing the equivalent continuous sound level.

### Deprecated Styles

static var discrete: HKQuantityAggregationStyle

Discrete samples may be averaged over time.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Quantity Type Data

var aggregationStyle: HKQuantityAggregationStyle

The aggregation style for the given quantity type.

func `is`(compatibleWith: HKUnit) -> Bool

Returns a Boolean value that indicates whether the quantity type is compatible with the given unit.

