

- DeviceActivity
- DeviceActivityReportScene
-  content 

Instance Property

# content

A closure that builds your report’s content with the provided configuration.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@ViewBuilder
var content: (Self.Configuration) -> Self.Content { get }
```

**Required**

## Discussion

Use this closure to update your scene’s content when your app changes the filter for a report or the system fetches more device activity data.

