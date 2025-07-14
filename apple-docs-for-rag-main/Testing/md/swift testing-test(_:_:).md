

- Swift Testing
-  Test(\_:\_:) 

Macro

# Test(\_:\_:)

Declare a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@attached(peer)
macro Test(
    _ displayName: String? = nil,
    _ traits: any TestTrait...
)
```

## Parameters 

`displayName`  

The customized display name of this test. If the value of this argument is `nil`, the display name of the test is derived from the associated function’s name.

`traits`  

Zero or more traits to apply to this test.

## See Also

### Related Documentation

Defining test functions

Define a test function to validate that code is working correctly.

### Essentials

Defining test functions

Define a test function to validate that code is working correctly.

Organizing test functions with suite types

Organize tests into test suites.

Migrating a test from XCTest

Migrate an existing test method or test class written using XCTest.

struct Test

A type representing a test or suite.

macro Suite(String?, any SuiteTrait...)

Declare a test suite.

