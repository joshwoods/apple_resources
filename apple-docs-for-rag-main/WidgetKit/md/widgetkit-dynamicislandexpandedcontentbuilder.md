

- WidgetKit
-  DynamicIslandExpandedContentBuilder 

Structure

# DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
@resultBuilder
struct DynamicIslandExpandedContentBuilder
```

## Topics

### Type Methods

static func buildPartialBlock&lt;C0, C1>(accumulated: DynamicIslandExpandedContent&lt;C0>, next: DynamicIslandExpandedContent&lt;C1>) -> DynamicIslandExpandedContent&lt;some View> 

static func buildPartialBlock&lt;C0, C1>(accumulated: DynamicIslandExpandedContent&lt;C0>, next: DynamicIslandExpandedRegion&lt;C1>) -> DynamicIslandExpandedContent&lt;some View> 

static func buildPartialBlock&lt;C>(first: DynamicIslandExpandedRegion&lt;C>) -> DynamicIslandExpandedContent&lt;some View> 

static func buildPartialBlock&lt;C>(first: DynamicIslandExpandedContent&lt;C>) -> DynamicIslandExpandedContent&lt;some View> 

## See Also

### Creating the expanded presentation

init(DynamicIslandExpandedRegionPosition, priority: Double, content: () -> Content)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

struct DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

