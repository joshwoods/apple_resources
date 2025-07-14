

- WidgetKit
- DynamicIslandExpandedRegion
-  init(\_:priority:content:) 

Initializer

# init(\_:priority:content:)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
init(
    _ position: DynamicIslandExpandedRegionPosition,
    priority: Double = 0,
    @ViewBuilder content: () -> Content
)
```

## Parameters 

`position`  

The position for Live Activity content.

`priority`  

The priority that tells the system which content to prioritize when it sizes the content of an expanded Live Activity in the Dynamic Island.

`content`  

The content of an expanded Live Activity.

## See Also

### Creating the expanded presentation

struct DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

