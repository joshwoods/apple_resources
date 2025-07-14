

- Swift Testing
- Test
-  isSuite 

Instance Property

# isSuite

Whether or not this instance is a test suite containing other tests.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var isSuite: Bool { get }
```

## Discussion

Instances of Test attached to types rather than functions are test suites. They do not contain any test logic of their own, but they may have traits added to them that also apply to their subtests.

A test suite can be declared using the Suite(_:_:) macro.

