

- Swift Testing
-  Suite(\_:\_:) 

Macro

# Suite(\_:\_:)

Declare a test suite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@attached(member) @attached(peer)
macro Suite(
    _ displayName: String? = nil,
    _ traits: any SuiteTrait...
)
```

## Parameters 

`displayName`  

The customized display name of this test suite. If the value of this argument is `nil`, the display name of the test is derived from the associated type’s name.

`traits`  

Zero or more traits to apply to this test suite.

## Overview

A test suite is a type that contains one or more test functions. Any copyable type (that is, any type that is not marked `~Copyable`) may be a test suite.

The use of the `@Suite` attribute is optional; types are recognized as test suites even if they do not have the `@Suite` attribute applied to them.

When adding test functions to a type extension, do not use the `@Suite` attribute. Only a type’s primary declaration may have the `@Suite` attribute applied to it.

## See Also

### Related Documentation

Organizing test functions with suite types

Organize tests into test suites.

### Essentials

Defining test functions

Define a test function to validate that code is working correctly.

Organizing test functions with suite types

Organize tests into test suites.

Migrating a test from XCTest

Migrate an existing test method or test class written using XCTest.

macro Test(String?, any TestTrait...)

Declare a test.

struct Test

A type representing a test or suite.

