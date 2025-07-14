

- Swift Testing
- Issue
- Issue.Kind
-  Issue.Kind.confirmationMiscounted(actual:expected:) 

Case

# Issue.Kind.confirmationMiscounted(actual:expected:)

An issue due to a confirmation being confirmed the wrong number of times.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
indirect case confirmationMiscounted(
    actual: Int,
    expected: any RangeExpression & Sendable
)
```

## Parameters 

`actual`  

The number of times confirm(count:) was actually called.

`expected`  

The expected number of times confirm(count:) should have been called.

## Discussion

This issue can occur when calling confirmation(_:expectedCount:isolation:sourceLocation:_:) or confirmation(_:expectedCount:isolation:sourceLocation:_:) when the confirmation passed to these functions’ `body` closures is confirmed too few or too many times.

