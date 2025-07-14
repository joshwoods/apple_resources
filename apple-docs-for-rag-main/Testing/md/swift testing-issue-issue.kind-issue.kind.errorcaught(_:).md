

- Swift Testing
- Issue
- Issue.Kind
-  Issue.Kind.errorCaught(\_:) 

Case

# Issue.Kind.errorCaught(\_:)

An issue due to an `Error` being thrown by a test function and caught by the testing library.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
indirect case errorCaught(any Error)
```

## Parameters 

`error`  

The error which was associated with this issue.

