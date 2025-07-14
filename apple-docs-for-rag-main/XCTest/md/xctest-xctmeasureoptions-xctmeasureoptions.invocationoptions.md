

- XCTest
- XCTMeasureOptions
-  XCTMeasureOptions.InvocationOptions 

Structure

# XCTMeasureOptions.InvocationOptions

Test measurement options that control how measurement starts and stops.

``` source
struct InvocationOptions
```

## Topics

### Measurement Options

static var manuallyStart: XCTMeasureOptions.InvocationOptions

An invocation option that specifies that the test starts taking measurements when the `startMeasuring()` function is called.

static var manuallyStop: XCTMeasureOptions.InvocationOptions

An invocation option that specifies that the test stops taking measurements when the `stopMeasuring()` function is called.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

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

### Using Option Details

var invocationOptions: XCTMeasureOptions.InvocationOptions

Options that define whether measurement is automatically or manually controlled.

var iterationCount: Int

The number of times the performance test measures its block.

