

- DeviceActivity
- DeviceActivityFilter
-  init(segment:devices:applications:categories:webDomains:) 

Initializer

# init(segment:devices:applications:categories:webDomains:)

Creates a new filter for the current user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
init(
    segment segmentInterval: DeviceActivityFilter.SegmentInterval = .hourly(),
    devices: DeviceActivityFilter.Devices? = nil,
    applications: Set = [],
    categories: Set = [],
    webDomains: Set = []
)
```

## Discussion

If you specify `applications`, `categories` or `webDomains`, then the system provides activity data for the requested application, categories, and web domains only. Conversely, if you do not specify any `applications`, `categories`, or `webDomains`, then the system provides data for all types of device activity. If you do not specify any `devices`, then the filter only includes data for the current device.

