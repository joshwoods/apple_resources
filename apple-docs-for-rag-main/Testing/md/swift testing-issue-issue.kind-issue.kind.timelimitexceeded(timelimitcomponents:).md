

- Swift Testing
- Issue
- Issue.Kind
-  Issue.Kind.timeLimitExceeded(timeLimitComponents:) 

Case

# Issue.Kind.timeLimitExceeded(timeLimitComponents:)

An issue due to a test reaching its time limit and timing out.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
indirect case timeLimitExceeded(timeLimitComponents: (seconds: Int64, attoseconds: Int64))
```

## Parameters 

`timeLimitComponents`  

The time limit reached by the test.

## Mentioned in 

Limiting the running time of tests

