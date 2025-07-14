

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
-  HKQuantitySeriesSampleQueryDescriptor.Options 

Structure

# HKQuantitySeriesSampleQueryDescriptor.Options

Options used when querying series data.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Options
```

## Topics

### Setting Options

static let includeSample: HKQuantitySeriesSampleQueryDescriptor.Options

An option indicating that the results should include a reference to the quantity sample that contains the series data.

static let orderByQuantitySampleStartDate: HKQuantitySeriesSampleQueryDescriptor.Options

An option indicating that the results are grouped by the containing quantity sample’s start date.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating Series Query Descriptors

init(predicate: HKSamplePredicate&lt;HKQuantitySample>, options: HKQuantitySeriesSampleQueryDescriptor.Options)

Creates a quantity series query descriptor.

