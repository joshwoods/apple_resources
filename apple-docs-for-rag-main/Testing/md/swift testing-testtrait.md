

- Swift Testing
-  TestTrait 

Protocol

# TestTrait

A protocol describing traits that can be added to a test function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
protocol TestTrait : Trait
```

## Overview

The testing library defines a number of traits that can be added to test functions. Developers can also define their own traits by creating types that conform to this protocol and/or to the SuiteTrait protocol.

## Relationships

### Inherits From

- Sendable
- Trait

### Conforming Types

- Bug
- Comment
- ConditionTrait
- ParallelizationTrait
- Tag.List
- TimeLimitTrait

## See Also

### Creating custom traits

protocol Trait

A protocol describing traits that can be added to a test function or to a test suite.

protocol SuiteTrait

A protocol describing traits that can be added to a test suite.

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

