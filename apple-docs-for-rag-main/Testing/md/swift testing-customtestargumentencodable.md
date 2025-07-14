

- Swift Testing
-  CustomTestArgumentEncodable 

Protocol

# CustomTestArgumentEncodable

A protocol for customizing how arguments passed to parameterized tests are encoded, which is used to match against when running specific arguments.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
protocol CustomTestArgumentEncodable : Sendable
```

## Mentioned in 

Implementing parameterized tests

## Overview

The testing library checks whether a test argument conforms to this protocol, or any of several other known protocols, when running selected test cases. When a test argument conforms to this protocol, that conformance takes highest priority, and the testing library will then call encodeTestArgument(to:) on the argument. A type that conforms to this protocol is not required to conform to either `Encodable` or `Decodable`.

See Implementing parameterized tests for a list of the other supported ways to allow running selected test cases.

## Topics

### Instance Methods

func encodeTestArgument(to: some Encoder) throws

Encode this test argument.

**Required**

## Relationships

### Inherits From

- Sendable

## See Also

### Related Documentation

Implementing parameterized tests

Specify different input parameters to generate multiple test cases from a test function.

### Test parameterization

Implementing parameterized tests

Specify different input parameters to generate multiple test cases from a test function.

macro Test&lt;C>(String?, any TestTrait..., arguments: C)

Declare a test parameterized over a collection of values.

macro Test&lt;C1, C2>(String?, any TestTrait..., arguments: C1, C2)

Declare a test parameterized over two collections of values.

macro Test&lt;C1, C2>(String?, any TestTrait..., arguments: Zip2Sequence&lt;C1, C2>)

Declare a test parameterized over two zipped collections of values.

struct Case

A single test case from a parameterized Test.

