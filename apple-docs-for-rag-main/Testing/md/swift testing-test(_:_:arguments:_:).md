

- Swift Testing
-  Test(\_:\_:arguments:\_:) 

Macro

# Test(\_:\_:arguments:\_:)

Declare a test parameterized over two collections of values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@attached(peer)
macro Test(
    _ displayName: String? = nil,
    _ traits: any TestTrait...,
    arguments collection1: C1,
    _ collection2: C2
) where C1 : Collection, C1 : Sendable, C2 : Collection, C2 : Sendable, C1.Element : Sendable, C2.Element : Sendable
```

## Parameters 

`displayName`  

The customized display name of this test. If the value of this argument is `nil`, the display name of the test is derived from the associated function’s name.

`traits`  

Zero or more traits to apply to this test.

`collection1`  

A collection of values to pass to `testFunction`.

`collection2`  

A second collection of values to pass to `testFunction`.

## Overview

During testing, the associated test function is called once for each pair of elements in `collection1` and `collection2`.

## See Also

### Related Documentation

Defining test functions

Define a test function to validate that code is working correctly.

### Test parameterization

Implementing parameterized tests

Specify different input parameters to generate multiple test cases from a test function.

macro Test&lt;C>(String?, any TestTrait..., arguments: C)

Declare a test parameterized over a collection of values.

macro Test&lt;C1, C2>(String?, any TestTrait..., arguments: Zip2Sequence&lt;C1, C2>)

Declare a test parameterized over two zipped collections of values.

protocol CustomTestArgumentEncodable

A protocol for customizing how arguments passed to parameterized tests are encoded, which is used to match against when running specific arguments.

struct Case

A single test case from a parameterized Test.

