

- XCTest
- XCTExpectedFailure
- XCTExpectedFailure.Options
-  nonStrict() 

Type Method

# nonStrict()

Options that specify that an unfulfilled expected failure doesn’t generate a test failure.

``` source
class func nonStrict() -> XCTExpectedFailure.Options
```

## Return Value

Returns an options instance that specifies that an unfulfilled expected failure doesn’t generate a test failure.

## See Also

### Specifying Options

var isEnabled: Bool

A Boolean value that indicates whether the test checks for the expected failure.

var isStrict: Bool

A Boolean value that indicates whether the test reports an error if the expected failure doesn’t occur.

