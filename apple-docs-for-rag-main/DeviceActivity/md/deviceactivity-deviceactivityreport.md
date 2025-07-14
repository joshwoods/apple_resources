

- DeviceActivity
-  DeviceActivityReport 

Structure

# DeviceActivityReport

A view that reports the user’s application, category, and web domain activity in a privacy-preserving way.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor @preconcurrency
struct DeviceActivityReport
```

## Overview

When you create a report, the system asks your app’s device activity report extension to provide a View representing the user’s device activity. To protect the user’s privacy, your extension runs in a sandbox. This sandbox prevents your extension from making network requests or moving sensitive content outside the extension’s address space. The extension point identifier for all device activity report extensions is `com.apple.deviceactivityui.report-extension`. You can configure a report with a custom context and filter, and then display the report like any SwiftUI view.

```
struct ExampleView: View {
    let selectedApps: Set
    let selectedCategories: Set
    let selectedWebDomains: Set

    @State private var context: DeviceActivityReport.Context = .barGraph
    @State private var filter = DeviceActivityFilter(
        segment: .daily(
            during: Calendar.current.dateInterval(
               of: .weekOfYear, for: .now
            )!
        ),
        users: .children,
        devices: .init([.iPhone, .iPad]),
        applications: selectedApps,
        categories: selectedCategories,
        webDomains: selectedWebDomains
    )

    public var body: some View {
        VStack {
            DeviceActivityReport(context, filter: filter)

            // A picker used to change the report's context.
            Picker(selection: $context, label: Text("Context: ")) {
                Text("Bar Graph")
                    .tag(DeviceActivityReport.Context.barGraph)
                Text("Pie Chart")
                     .tag(DeviceActivityReport.Context.pieChart)
            }

            // A picker used to change the filter's segment interval.
            Picker(
                selection: $filter.segmentInterval,
                 label: Text("Segment Interval: ")
            ) {
                Text("Hourly")
                    .tag(DeviceActivityFilter.SegmentInterval.hourly())
                Text("Daily")
                    .tag(DeviceActivityFilter.SegmentInterval.daily(
                        during: Calendar.current.dateInterval(
                             of: .weekOfYear, for: .now
                        )!
                    ))
                Text("Weekly")
                    .tag(DeviceActivityFilter.SegmentInterval.weekly(
                        during: Calendar.current.dateInterval(
                            of: .month, for: .now
                        )!
                    ))
            }
            // ...
        }
    }
}
```

The system will only provide your extension with device activity data if the user has authorized your app for family controls on their device or on the device(s) of children in their iCloud family. See AuthorizationCenter for more details.

## Topics

### Structures

struct Context

A context indicating how your device activity report extension should configure its `DeviceActivityReportView`.

### Initializers

init(DeviceActivityReport.Context, filter: DeviceActivityFilter)

Creates a new device activity report.

### Instance Properties

var body: some View

The content of the device activity report.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

