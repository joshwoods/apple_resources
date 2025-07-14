

- WidgetKit
- DynamicIsland
-  init(expanded:compactLeading:compactTrailing:minimal:) 

Initializer

# init(expanded:compactLeading:compactTrailing:minimal:)

Creates a configuration object with views that appear in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
init(
    @DynamicIslandExpandedContentBuilder expanded: @escaping () -> DynamicIslandExpandedContent,
    @ViewBuilder compactLeading: @escaping () -> CompactLeading,
    @ViewBuilder compactTrailing: @escaping () -> CompactTrailing,
    @ViewBuilder minimal: @escaping () -> Minimal
) where Expanded : View, CompactLeading : View, CompactTrailing : View, Minimal : View
```

## Parameters 

`expanded`  

A closure that builds the view for the expanded presentation of the Live Activity.

`compactLeading`  

A closure that builds the view for the compact leading presentation of the Live Activity.

`compactTrailing`  

A closure that builds the view for the compact trailing presentation of the Live Activity.

`minimal`  

A closure that builds the view for the minimal presentation of the Live Activity.

## See Also

### Creating the view for the Dynamic Island

struct DynamicIslandExpandedRegion

A structure that defines and positions the content of an expanded Live Activity in the Dynamic Island.

