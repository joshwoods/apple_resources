

- Swift
- Duration
-  init(secondsComponent:attosecondsComponent:) 

Initializer

# init(secondsComponent:attosecondsComponent:)

Construct a `Duration` by adding attoseconds to a seconds value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    secondsComponent: Int64,
    attosecondsComponent: Int64
)
```

## Parameters 

`secondsComponent`  

The seconds component portion of the `Duration` value.

`attosecondsComponent`  

The attosecond component portion of the `Duration` value.

## Discussion

This is useful for when an external decomposed components of a `Duration` has been stored and needs to be reconstituted. Since the values are added no precondition is expressed for the attoseconds being limited to 1e18.

```
  let d1 = Duration(
    secondsComponent: 3, 
    attosecondsComponent: 123000000000000000)
  print(d1) // 3.123 seconds

  let d2 = Duration(
    secondsComponent: 3, 
    attosecondsComponent: -123000000000000000)
  print(d2) // 2.877 seconds

  let d3 = Duration(
    secondsComponent: -3, 
    attosecondsComponent: -123000000000000000)
  print(d3) // -3.123 seconds
```

## See Also

### Creating a duration

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

