

- XCTest
- XCTExpectedFailure
- XCTExpectedFailure.Options
-  isStrict 

Instance Property

# isStrict

A Boolean value that indicates whether the test reports an error if the expected failure doesn’t occur.

``` source
var isStrict: Bool { get set }
```

## Discussion

The default is `true`. Set this property to `false` to prevent the test from recording the unfilled expected failure as an issue.

## See Also

### Specifying Options

class func nonStrict() -> XCTExpectedFailure.Options

Options that specify that an unfulfilled expected failure doesn’t generate a test failure.

var isEnabled: Bool

A Boolean value that indicates whether the test checks for the expected failure.

