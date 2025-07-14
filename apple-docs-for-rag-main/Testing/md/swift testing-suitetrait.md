

- Swift Testing
-  SuiteTrait 

Protocol

# SuiteTrait

A protocol describing traits that can be added to a test suite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
protocol SuiteTrait : Trait
```

## Overview

The testing library defines a number of traits that can be added to test suites. Developers can also define their own traits by creating types that conform to this protocol and/or to the TestTrait protocol.

## Topics

### Instance Properties

var isRecursive: Bool

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

**Required** Default implementation provided.

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

protocol TestTrait

A protocol describing traits that can be added to a test function.

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

