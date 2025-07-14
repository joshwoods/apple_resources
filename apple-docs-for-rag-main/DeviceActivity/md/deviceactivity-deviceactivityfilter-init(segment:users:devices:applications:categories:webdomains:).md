

- DeviceActivity
- DeviceActivityFilter
-  init(segment:users:devices:applications:categories:webDomains:) 

Initializer

# init(segment:users:devices:applications:categories:webDomains:)

Creates a new filter for the specified users and devices.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
init(
    segment segmentInterval: DeviceActivityFilter.SegmentInterval = .hourly(),
    users: DeviceActivityFilter.Users,
    devices: DeviceActivityFilter.Devices,
    applications: Set = [],
    categories: Set = [],
    webDomains: Set = []
)
```

## Discussion

If you specify `applications`, `categories` or `webDomains`, then the system provides activity data for the requested application, categories, and web domains only. Conversely, if you do not specify any `applications`, `categories`, or `webDomains`, then the system provides data for all types of device activity.

