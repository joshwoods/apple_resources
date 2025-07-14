

- HealthKit
-  HKMetricPrefix 

Enumeration

# HKMetricPrefix

Prefixes that can be added to SI units to change the order of magnitude.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKMetricPrefix
```

## Topics

### Prefixes

case none

A prefix that does not modify the base unit.

case femto

A prefix that multiplies the base unit by 1e-15.

case pico

A prefix that multiplies the base unit by 1e-12.

case nano

A prefix that multiplies the base unit by 1e-9.

case micro

A prefix that multiplies the base unit by 1e-6.

case milli

A prefix that multiplies the base unit by 0.001.

case centi

A prefix that multiplies the base unit by 0.01.

case deci

A prefix that multiplies the base unit by 0.1.

case deca

A prefix that multiplies the base unit by 10.

case hecto

A prefix that multiplies the base unit by 100.

case kilo

A prefix that multiplies the base unit by 1000.

case mega

A prefix that multiplies the base unit by 1e6.

case giga

A prefix that multiplies the base unit by 1e9.

case tera

A prefix that multiplies the base unit by 1e12.

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

### Units and quantities

Defining and converting units and quantities

Create and convert units and quantities.

class HKQuantity

An object that stores a value for a given unit.

class HKUnit

A class for managing the units of measure within HealthKit.

