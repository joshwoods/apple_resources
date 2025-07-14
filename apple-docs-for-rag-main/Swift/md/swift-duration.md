

- Swift
-  Duration 

Structure

# Duration

A representation of high precision time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct Duration
```

## Overview

`Duration` represents an elapsed time value with high precision in an integral form. It may be used for measurements of varying clock sources. In those cases it represents the elapsed time measured by that clock. Calculations using `Duration` may span from a negative value to a positive value and have a suitable range to at least cover attosecond scale for both small elapsed durations like sub-second precision to durations that span centuries.

Typical construction of `Duration` values should be created via the static methods for specific time values.

```
 var d: Duration = .seconds(3)
 d += .milliseconds(33)
 print(d) // 3.033 seconds
```

`Duration` itself does not ferry any additional information other than the temporal measurement component; specifically leap seconds should be represented as an additional accessor since that is specific only to certain clock implementations.

## Topics

### Creating a duration

init(secondsComponent: Int64, attosecondsComponent: Int64)

Construct a `Duration` by adding attoseconds to a seconds value.

static func seconds&lt;T>(T) -> Duration

Construct a `Duration` given a number of seconds represented as a `BinaryInteger`.

static func seconds(Double) -> Duration

Construct a `Duration` given a number of seconds represented as a `Double` by converting the value into the closest attosecond scale value.

static func milliseconds&lt;T>(T) -> Duration

Construct a `Duration` given a number of milliseconds represented as a `BinaryInteger`.

static func milliseconds(Double) -> Duration

Construct a `Duration` given a number of seconds milliseconds as a `Double` by converting the value into the closest attosecond scale value.

static func microseconds(Double) -> Duration

Construct a `Duration` given a number of seconds microseconds as a `Double` by converting the value into the closest attosecond scale value.

static func microseconds&lt;T>(T) -> Duration

Construct a `Duration` given a number of microseconds represented as a `BinaryInteger`.

static func nanoseconds&lt;T>(T) -> Duration

Construct a `Duration` given a number of nanoseconds represented as a `BinaryInteger`.

### Accessing a duration’s components

var components: (seconds: Int64, attoseconds: Int64)

The composite components of the `Duration`.

### Performing calculations on durations

static func * (Duration, Double) -> Duration

static func *= &lt;T>(inout Duration, T)

static func / (Duration, Double) -> Duration

static func /= (inout Duration, Double)

static func /= &lt;T>(inout Duration, T)

### Formatting a duration

func formatted() -> String

Formats the string using a localized hour-minute-second time pattern.

func formatted&lt;S>(S) -> S.FormatOutput

Formats the duration, using the provided format style.

struct TimeFormatStyle

A format style that shows durations in a compact, localized format with separators.

struct UnitsFormatStyle

A format style that shows durations with localized labeled components

### Initializers

init(timeval)

### Default Implementations

AdditiveArithmetic Implementations

AtomicRepresentable Implementations

Comparable Implementations

CustomStringConvertible Implementations

Decodable Implementations

DurationProtocol Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- AtomicRepresentable
- BitwiseCopyable
- Comparable
- Copyable
- CustomStringConvertible
- Decodable
- DurationProtocol
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Durations

protocol DurationProtocol

A type that defines a duration for a given `InstantProtocol` type.

