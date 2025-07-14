

- DeviceActivity
- DeviceActivityEvent
-  init(applications:categories:webDomains:threshold:includesPastActivity:) 

Initializer

# init(applications:categories:webDomains:threshold:includesPastActivity:)

Creates a new event.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
init(
    applications: Set = [],
    categories: Set = [],
    webDomains: Set = [],
    threshold: DateComponents,
    includesPastActivity: Bool
)
```

## Parameters 

`applications`  

An optional list of applications to include in the event. A small subset of popular App Store apps have known associated web domains that get included implicitly. For example, an event that includes an app implicitly includes usage of the app’s web domain.

`categories`  

An optional list of categories to include in the event.

`webDomains`  

An optional list of web domains to include in the event. Some web domains have associated apps included implicitly.

`threshold`  

The amount of time that results in a callback to a DeviceActivityMonitor.

`includesPastActivity`  

Whether the system takes into account the person’s device activity before your app starts monitoring the event. For example, if your app calls startMonitoring(_:during:events:) at 1:30pm with a schedule of 1:00pm to 2:00pm, then this boolean determines whether any activity between 1:00 PM and 1:30 PM will contribute to its threshold.

## Discussion

An application’s extension receives a callback once the combination of specified applications, categories, and webDomains have been in use longer than the event’s threshold within the activity’s scheduled interval. If your app didn’t specify any `applications`, `categories`, or `webDomains`, the event includes all `applications`, `categories`, and `web domains`.

