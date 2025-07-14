

- Swift Testing
- Test
-  Test.Case 

Structure

# Test.Case

A single test case from a parameterized Test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Case
```

## Overview

A test case represents a test run with a particular combination of inputs. Tests that are *not* parameterized map to a single instance of Test.Case.

## Topics

### Instance Properties

var isParameterized: Bool

Whether or not this test case is from a parameterized test.

### Type Properties

static var current: Test.Case?

The test case that is running on the current task, if any.

## Relationships

### Conforms To

- Sendable

## See Also

### Test parameterization

Implementing parameterized tests

Specify different input parameters to generate multiple test cases from a test function.

macro Test&lt;C>(String?, any TestTrait..., arguments: C)

Declare a test parameterized over a collection of values.

macro Test&lt;C1, C2>(String?, any TestTrait..., arguments: C1, C2)

Declare a test parameterized over two collections of values.

macro Test&lt;C1, C2>(String?, any TestTrait..., arguments: Zip2Sequence&lt;C1, C2>)

Declare a test parameterized over two zipped collections of values.

protocol CustomTestArgumentEncodable

A protocol for customizing how arguments passed to parameterized tests are encoded, which is used to match against when running specific arguments.

