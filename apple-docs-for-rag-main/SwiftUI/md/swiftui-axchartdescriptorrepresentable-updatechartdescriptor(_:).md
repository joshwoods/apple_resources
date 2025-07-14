

- SwiftUI
- AXChartDescriptorRepresentable
-  updateChartDescriptor(\_:) 

Instance Method

# updateChartDescriptor(\_:)

Update the existing `AXChartDescriptor` for your view, based on changes in your view or in the `Environment`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func updateChartDescriptor(_ descriptor: AXChartDescriptor)
```

**Required** Default implementation provided.

## Discussion

This will be called as needed, when accessibility needs your `AXChartDescriptor` for VoiceOver. It will only be called if the inputs to your views, or a relevant part of the `Environment`, have changed.

## Default Implementations

### AXChartDescriptorRepresentable Implementations

func updateChartDescriptor(AXChartDescriptor)

Update the existing `AXChartDescriptor` for your view, based on changes in your view or in the `Environment`.

## See Also

### Managing a descriptor

func makeChartDescriptor() -> AXChartDescriptor

Create the `AXChartDescriptor` for this view, and return it.

**Required**

