

- XCTest
-  XCTMeasureOptions 

Class

# XCTMeasureOptions

Options to control the gathering of performance measurements during tests.

``` source
class XCTMeasureOptions
```

## Topics

### Getting Default Options

class var `default`: XCTMeasureOptions

The default measurement options.

### Using Option Details

var invocationOptions: XCTMeasureOptions.InvocationOptions

Options that define whether measurement is automatically or manually controlled.

struct InvocationOptions

Test measurement options that control how measurement starts and stops.

var iterationCount: Int

The number of times the performance test measures its block.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

