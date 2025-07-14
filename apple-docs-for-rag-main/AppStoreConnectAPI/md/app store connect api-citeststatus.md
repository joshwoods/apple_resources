

- App Store Connect API
-  CiTestStatus 

Type

# CiTestStatus

A string that represents test status information.

App Store Connect API 1.5+

``` source
string CiTestStatus
```

## Possible Values 

`SUCCESS`  

`FAILURE`  

`MIXED`  

`SKIPPED`  

`EXPECTED_FAILURE`  

## Possible Values

SUCCESS  
The tests passed.

FAILURE  
The tests failed.

MIXED  
Some tests passed and some failed.

SKIPPED  
Xcode Cloud skipped some tests.

EXPECTED_FAILURE  
Tests failed that you marked as expected to fail with \[XCTExpectFailure\](https://developer.apple.com/documentation/xctest/3726077- termxctexpectfailure).

## See Also

### Objects and Types

object CiTestResult.Attributes.DestinationTestResults

The results of a test action Xcode Cloud performed using a specific test destination.

