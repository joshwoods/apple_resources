

- Swift Testing
-  Expectation 

Structure

# Expectation

A type describing an expectation that has been evaluated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Expectation
```

## Topics

### Instance Properties

var isPassing: Bool

Whether the expectation passed or failed.

var isRequired: Bool

Whether or not the expectation was required to pass.

var sourceLocation: SourceLocation

The source location where this expectation was evaluated.

## Relationships

### Conforms To

- Sendable

## See Also

### Retrieving information about checked expectations

struct ExpectationFailedError

A type describing an error thrown when an expectation fails during evaluation.

protocol CustomTestStringConvertible

A protocol describing types with a custom string representation when presented as part of a test’s output.

