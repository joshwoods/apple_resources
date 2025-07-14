

- Swift Testing
-  ExpectationFailedError 

Structure

# ExpectationFailedError

A type describing an error thrown when an expectation fails during evaluation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct ExpectationFailedError
```

## Overview

The testing library throws instances of this type when the `#require()` macro records an issue.

## Topics

### Instance Properties

var expectation: Expectation

The expectation that failed.

## Relationships

### Conforms To

- Error
- Sendable

## See Also

### Retrieving information about checked expectations

struct Expectation

A type describing an expectation that has been evaluated.

protocol CustomTestStringConvertible

A protocol describing types with a custom string representation when presented as part of a test’s output.

