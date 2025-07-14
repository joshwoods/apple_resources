

- Swift Testing
- Test
- Test.ID
-  parent 

Instance Property

# parent

The ID of the parent test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var parent: Test.ID? { get }
```

## Discussion

If this test’s ID has no parent (i.e. the test is at the root of a test graph), the value of this property is `nil`.

