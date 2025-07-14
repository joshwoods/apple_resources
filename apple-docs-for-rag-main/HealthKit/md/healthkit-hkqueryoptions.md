

- HealthKit
-  HKQueryOptions 

Structure

# HKQueryOptions

Constants that describe how a sample’s time period overlaps with the target time period.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
struct HKQueryOptions
```

## Topics

### Constants

static var strictStartDate: HKQueryOptions

The sample’s start time must fall within the target time period.

static var strictEndDate: HKQueryOptions

The sample’s end time must fall within the target time period.

### Initializers

init(rawValue: UInt)

Returns a newly initialized query option using the provided integer.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating sample predicates

class func predicateForSamples(withStart: Date?, end: Date?, options: HKQueryOptions) -> NSPredicate

Returns a predicate for samples whose start and end dates fall within the specified time interval.

