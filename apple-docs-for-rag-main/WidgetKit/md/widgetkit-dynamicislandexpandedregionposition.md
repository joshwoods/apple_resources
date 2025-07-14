

- WidgetKit
-  DynamicIslandExpandedRegionPosition 

Structure

# DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIslandExpandedRegionPosition
```

## Topics

### View positions

static let bottom: DynamicIslandExpandedRegionPosition

The bottom position in the Dynamic Island for views of an expanded Live Activity.

static let center: DynamicIslandExpandedRegionPosition

The center position in the Dynamic Island for views of an expanded Live Activity.

static let leading: DynamicIslandExpandedRegionPosition

The leading position in the Dynamic Island for views of an expanded Live Activity.

static let trailing: DynamicIslandExpandedRegionPosition

The trailing position in the Dynamic Island for views of an expanded Live Activity.

## See Also

### Creating the expanded presentation

init(DynamicIslandExpandedRegionPosition, priority: Double, content: () -> Content)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

struct DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

