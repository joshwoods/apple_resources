

- DeviceActivity
- DeviceActivityReportScene
-  makeConfiguration(representing:) 

Instance Method

# makeConfiguration(representing:)

Creates a new configuration that represents the provided data.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func makeConfiguration(representing data: DeviceActivityResults) async -> Self.Configuration
```

**Required**

## Discussion

Use this function to create a new configuration when your app changes the filter for a report or the system fetches more device activity data.

