

- Matter
- MTRBaseClusterThermostat
-  setActiveScheduleRequestWith(\_:completion:) 

Instance Method

# setActiveScheduleRequestWith(\_:completion:)

Command SetActiveScheduleRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setActiveScheduleRequestWith(
    _ params: MTRThermostatClusterSetActiveScheduleRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func setActiveScheduleRequestWith(_ params: MTRThermostatClusterSetActiveScheduleRequestParams) async throws
```

## Discussion

Upon receipt, if the Schedules attribute contains a ScheduleStruct whose ScheduleHandle field matches the value of the ScheduleHandle field, the server SHALL set the thermostat’s ActiveScheduleHandle attribute to the value of the ScheduleHandle field.

