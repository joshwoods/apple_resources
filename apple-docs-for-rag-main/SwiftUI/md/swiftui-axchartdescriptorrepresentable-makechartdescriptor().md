

- SwiftUI
- AXChartDescriptorRepresentable
-  makeChartDescriptor() 

Instance Method

# makeChartDescriptor()

Create the `AXChartDescriptor` for this view, and return it.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func makeChartDescriptor() -> AXChartDescriptor
```

**Required**

## Discussion

This will be called once per identity of your `View`. It will not be run again unless the identity of your `View` changes. If you need to update the `AXChartDescriptor` based on changes in your `View`, or in the `Environment`, implement `updateChartDescriptor`. This method will only be called if / when accessibility needs the `AXChartDescriptor` of your view, for VoiceOver.

## See Also

### Managing a descriptor

func updateChartDescriptor(AXChartDescriptor)

Update the existing `AXChartDescriptor` for your view, based on changes in your view or in the `Environment`.

**Required** Default implementation provided.

