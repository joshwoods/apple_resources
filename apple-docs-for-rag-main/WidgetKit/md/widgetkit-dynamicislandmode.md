

- WidgetKit
-  DynamicIslandMode 

Structure

# DynamicIslandMode

A structure that offers values that describe the content mode for a Live Activity.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIslandMode
```

## Topics

### Dynamic Island presentations

static let compactLeading: DynamicIslandMode

The compact leading presentation of a Live Activity in the Dynamic Island.

static let compactTrailing: DynamicIslandMode

The compact trailing presentation of a Live Activity in the Dynamic Island.

static let expanded: DynamicIslandMode

The expanded presentation of a Live Activity in the Dynamic Island.

static let minimal: DynamicIslandMode

The minimal presentation of a Live Activity in the Dynamic Island.

## Relationships

### Conforms To

- Equatable

## See Also

### Specifying content margins

func contentMargins(Edge.Set, Double, for: DynamicIslandMode) -> DynamicIsland

Overrides default content margins for the provided content modes in the Dynamic Island.

