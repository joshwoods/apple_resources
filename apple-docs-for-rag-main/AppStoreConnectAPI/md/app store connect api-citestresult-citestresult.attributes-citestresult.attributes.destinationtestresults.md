

- App Store Connect API
- CiTestResult
- CiTestResult.Attributes
-  CiTestResult.Attributes.DestinationTestResults 

Object

# CiTestResult.Attributes.DestinationTestResults

The results of a test action Xcode Cloud performed using a specific test destination.

App Store Connect API 1.5+

``` source
object CiTestResult.Attributes.DestinationTestResults
```

## Properties

`deviceName`

`string`

The name of the simulated device used for tests.

`duration`

`number`

The time it took to perform a test on a specific simulated device.

`osVersion`

`string`

The OS version of the simulated device that Xcode Cloud used to run a test.

`status`

CiTestStatus

The status of a test for a specific simulated device.

`uuid`

`string`

The unique identifier of a test result for a specific simulated device.

## See Also

### Objects and Types

type CiTestStatus

A string that represents test status information.

