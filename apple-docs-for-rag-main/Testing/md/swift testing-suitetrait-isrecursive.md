

- Swift Testing
- SuiteTrait
-  isRecursive 

Instance Property

# isRecursive

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var isRecursive: Bool { get }
```

**Required** Default implementation provided.

## Discussion

By default, traits are not recursively applied to children.

## Default Implementations

### SuiteTrait Implementations

var isRecursive: Bool

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

