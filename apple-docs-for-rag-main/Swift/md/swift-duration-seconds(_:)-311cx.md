

- Swift
- Duration
-  seconds(\_:) 

Type Method

# seconds(\_:)

Construct a `Duration` given a number of seconds represented as a `BinaryInteger`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func seconds(_ seconds: T) -> Duration where T : BinaryInteger
```

## Return Value

A `Duration` representing a given number of seconds.

## Discussion

```
  let d: Duration = .seconds(77)
```

## See Also

### Creating a duration

init(secondsComponent: Int64, attosecondsComponent: Int64)

Construct a `Duration` by adding attoseconds to a seconds value.

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

