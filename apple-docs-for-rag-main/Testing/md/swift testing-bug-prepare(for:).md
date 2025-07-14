

- Swift Testing
- Bug
-  prepare(for:) 

Instance Method

# prepare(for:)

Prepare to run the test to which this trait was added.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
func prepare(for test: Test) async throws
```

## Parameters 

`test`  

The test to which this trait was added.

## Discussion

Throws

Any error that would prevent the test from running. If an error is thrown from this method, the test will be skipped and the error will be recorded as an Issue.

This method is called after all tests and their traits have been discovered by the testing library, but before any test has begun running. It may be used to prepare necessary internal state, or to influence whether the test should run.

The default implementation of this method does nothing.

