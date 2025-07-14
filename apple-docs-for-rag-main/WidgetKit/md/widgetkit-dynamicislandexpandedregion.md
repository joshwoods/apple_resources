

- WidgetKit
-  DynamicIslandExpandedRegion 

Structure

# DynamicIslandExpandedRegion

A structure that defines and positions the content of an expanded Live Activity in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIslandExpandedRegion where Content : View
```

## Overview

The expanded presentation of a Live Activity in the Dynamic Island consists of four regions:

- center places content right below the TrueDepth camera.

- leading places content along the leading edge of the expanded Live Activity next to the TrueDepth camera and wraps additional content below it.

- trailing places content along the trailing edge of the expanded Live Activity next to the TrueDepth camera and wraps additional content below it.

- bottom places content below leading, trailing, and center content.

## Topics

### Creating the expanded presentation

init(DynamicIslandExpandedRegionPosition, priority: Double, content: () -> Content)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

struct DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

### Specifying custom content margins

func contentMargins(Edge.Set, Double) -> DynamicIslandExpandedRegion&lt;Content>

Overrides default content margins for the provided edges in the Dynamic Island.

## See Also

### Creating the view for the Dynamic Island

init&lt;Expanded, CompactLeading, CompactTrailing, Minimal>(expanded: () -> DynamicIslandExpandedContent&lt;Expanded>, compactLeading: () -> CompactLeading, compactTrailing: () -> CompactTrailing, minimal: () -> Minimal)

Creates a configuration object with views that appear in the Dynamic Island.

