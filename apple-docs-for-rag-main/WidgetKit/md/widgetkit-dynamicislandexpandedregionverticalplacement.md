

- WidgetKit
-  DynamicIslandExpandedRegionVerticalPlacement 

Structure

# DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIslandExpandedRegionVerticalPlacement
```

## Topics

### Configuring vertical content placement

static let `default`: DynamicIslandExpandedRegionVerticalPlacement

The system’s default vertical placement.

static let belowIfTooWide: DynamicIslandExpandedRegionVerticalPlacement

Vertical placement below the default vertical position for content that’s too wide to fit next to the TrueDepth camera.

## Relationships

### Conforms To

- Equatable

## See Also

### Creating the expanded presentation

init(DynamicIslandExpandedRegionPosition, priority: Double, content: () -> Content)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

struct DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

