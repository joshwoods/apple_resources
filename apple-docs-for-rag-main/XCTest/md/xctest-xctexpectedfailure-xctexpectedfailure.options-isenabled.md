

- XCTest
- XCTExpectedFailure
- XCTExpectedFailure.Options
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the test checks for the expected failure.

``` source
var isEnabled: Bool { get set }
```

## Discussion

The default is `true`. Set this property to `false` to disable the expected failure check.

## See Also

### Specifying Options

class func nonStrict() -> XCTExpectedFailure.Options

Options that specify that an unfulfilled expected failure doesn’t generate a test failure.

var isStrict: Bool

A Boolean value that indicates whether the test reports an error if the expected failure doesn’t occur.

