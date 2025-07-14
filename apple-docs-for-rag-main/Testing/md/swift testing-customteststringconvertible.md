

- Swift Testing
-  CustomTestStringConvertible 

Protocol

# CustomTestStringConvertible

A protocol describing types with a custom string representation when presented as part of a test’s output.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
protocol CustomTestStringConvertible
```

## Overview

Values whose types conform to this protocol use it to describe themselves when they are present as part of the output of a test. For example, this protocol affects the display of values that are passed as arguments to test functions or that are elements of an expectation failure.

By default, the testing library converts values to strings using `String(describing:)`. The resulting string may be inappropriate for some types and their values. If the type of the value is made to conform to CustomTestStringConvertible, then the value of its testDescription property will be used instead.

For example, consider the following type:

```
enum Food: CaseIterable {
  case paella, oden, ragu
}
```

If an array of cases from this enumeration is passed to a parameterized test function:

```
@Test(arguments: Food.allCases)
func isDelicious(_ food: Food) { ... }
```

Then the values in the array need to be presented in the test output, but the default description of a value may not be adequately descriptive:

```
◇ Passing argument food → .paella to isDelicious(_:)
◇ Passing argument food → .oden to isDelicious(_:)
◇ Passing argument food → .ragu to isDelicious(_:)
```

By adopting CustomTestStringConvertible, customized descriptions can be included:

```
extension Food: CustomTestStringConvertible {
  var testDescription: String {
    switch self {
    case .paella:
      "paella valenciana"
    case .oden:
      "おでん"
    case .ragu:
      "ragù alla bolognese"
    }
  }
}
```

The presentation of these values will then reflect the value of the testDescription property:

```
◇ Passing argument food → paella valenciana to isDelicious(_:)
◇ Passing argument food → おでん to isDelicious(_:)
◇ Passing argument food → ragù alla bolognese to isDelicious(_:)
```

## Topics

### Instance Properties

var testDescription: String

A description of this instance to use when presenting it in a test’s output.

**Required** Default implementation provided.

## See Also

### Retrieving information about checked expectations

struct Expectation

A type describing an expectation that has been evaluated.

struct ExpectationFailedError

A type describing an error thrown when an expectation fails during evaluation.

