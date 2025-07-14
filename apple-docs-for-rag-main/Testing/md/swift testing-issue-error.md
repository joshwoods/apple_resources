

- Swift Testing
- Issue
-  error 

Instance Property

# error

The error which was associated with this issue, if any.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var error: (any Error)? { get }
```

## Discussion

The value of this property is non-`nil` when kind is Issue.Kind.errorCaught(_:).

