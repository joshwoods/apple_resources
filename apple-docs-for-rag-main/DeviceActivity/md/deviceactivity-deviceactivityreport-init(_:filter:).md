

- DeviceActivity
- DeviceActivityReport
-  init(\_:filter:) 

Initializer

# init(\_:filter:)

Creates a new device activity report.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
init(
    _ context: DeviceActivityReport.Context,
    filter: DeviceActivityFilter = DeviceActivityFilter()
)
```

## Parameters 

`context`  

The context of the report.

`filter`  

A filter for the device activity data that your app extension will use to render the report.

## Discussion

If you do not specify a filter, then the system will provide all device activity data for the current user and the current device to your device activity report app extension.

