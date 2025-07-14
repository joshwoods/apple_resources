

- WidgetKit
-  DynamicIslandExpandedContent 

Structure

# DynamicIslandExpandedContent

A view that describes the expanded presentation of a Live Activity that appears in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIslandExpandedContent where Content : View
```

## Overview

This view holds the intermediate content for the DynamicIslandExpandedContentBuilder.

## See Also

### Creating the expanded presentation

init(DynamicIslandExpandedRegionPosition, priority: Double, content: () -> Content)

Creates the object that defines and positions the content of an expanded Live Activity in the Dynamic Island.

struct DynamicIslandExpandedRegionPosition

View positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedRegionVerticalPlacement

Vertical view positions of an expanded Live Activity that appears in the Dynamic Island.

struct DynamicIslandExpandedContentBuilder

A result builder that constructs the content of an expanded Live Activity in the Dynamic Island.

