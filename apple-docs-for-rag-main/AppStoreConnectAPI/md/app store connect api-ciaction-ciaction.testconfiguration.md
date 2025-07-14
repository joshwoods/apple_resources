

- App Store Connect API
- CiAction
-  CiAction.TestConfiguration 

Object

# CiAction.TestConfiguration

The test configuration for a test action.

App Store Connect API 1.5+

``` source
object CiAction.TestConfiguration
```

## Properties

`kind`

`string`

A string that describes whether the test action uses the scheme’s default tests or a specific test plan.

Possible Values: `USE_SCHEME_SETTINGS, SPECIFIC_TEST_PLANS`

`testDestinations`

`[`CiTestDestination`]`

A list of destination information for the test configuration.

`testPlanName`

`string`

The name of the test plan. This value is only available to test actions that set the `kind` field to `SPECIFIC_TEST_PLANS`.

## Topics

### Objects and Types

object CiTestDestination

The test destination of a test action that Xcode Cloud performs.

type CiTestDestinationKind

The string that represents the kind of a test destination.

