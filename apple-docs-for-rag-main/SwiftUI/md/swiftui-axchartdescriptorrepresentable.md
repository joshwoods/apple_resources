

- SwiftUI
-  AXChartDescriptorRepresentable 

Protocol

# AXChartDescriptorRepresentable

A type to generate an `AXChartDescriptor` object that you use to provide information about a chart and its data for an accessible experience in VoiceOver or other assistive technologies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AXChartDescriptorRepresentable
```

## Overview

Note that you may use the `@Environment` property wrapper inside the implementation of your `AXChartDescriptorRepresentable`, in which case you should implement `updateChartDescriptor`, which will be called when the `Environment` changes.

For example, to provide accessibility for a view that represents a chart, you would first declare your chart descriptor representable type:

```
struct MyChartDescriptorRepresentable: AXChartDescriptorRepresentable {
    func makeChartDescriptor() -> AXChartDescriptor {
        // Build and return your `AXChartDescriptor` here.
    }

    func updateChartDescriptor(_ descriptor: AXChartDescriptor) {
        // Update your chart descriptor with any new values.
    }
}
```

Then, provide an instance of your `AXChartDescriptorRepresentable` type to your view using the `accessibilityChartDescriptor` modifier:

```
var body: some View {
    MyChartView()
        .accessibilityChartDescriptor(MyChartDescriptorRepresentable())
}
```

## Topics

### Managing a descriptor

func makeChartDescriptor() -> AXChartDescriptor

Create the `AXChartDescriptor` for this view, and return it.

**Required**

func updateChartDescriptor(AXChartDescriptor)

Update the existing `AXChartDescriptor` for your view, based on changes in your view or in the `Environment`.

**Required** Default implementation provided.

## See Also

### Describing charts

func accessibilityChartDescriptor&lt;R>(R) -> some View

Adds a descriptor to a View that represents a chart to make the chart’s contents accessible to all users.

