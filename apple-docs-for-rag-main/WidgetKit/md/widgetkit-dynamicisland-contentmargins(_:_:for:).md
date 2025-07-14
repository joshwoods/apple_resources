

- WidgetKit
- DynamicIsland
-  contentMargins(\_:\_:for:) 

Instance Method

# contentMargins(\_:\_:for:)

Overrides default content margins for the provided content modes in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
func contentMargins(
    _ edges: Edge.Set = .all,
    _ length: Double,
    for mode: DynamicIslandMode
) -> DynamicIsland
```

## Parameters 

`edges`  

The edges that should use custom content margins.

`length`  

The value for the custom content margin for the specified `edges`.

`mode`  

The presentation of the Dynamic Island that the custom content margins apply to.

## Return Value

The Dynamic Island view with updated content margins.

## Discussion

Use this modifier to customize the content margins for a content mode in the Dynamic Island. Avoid placing content too close to the edges of the Dynamic Island.

The following example uses the default margin for the leading edge and sets a custom margin of 8 points for the top, bottom, and trailing edges of a Live Activity in the expanded presentation:

```
dynamicIsland
    .contentMargins([.top, .bottom, .trailing], 8, for:.expanded)
```

When you apply multiple `contentMargins(_:_:for:)` modifiers, modifiers with the same placement override modifiers higher up in the view hierarchy. The following example results in a margin of 8 points for the trailing edge and 20 points for all other edges when the Live Activity appears in the expanded presentation:

```
dynamicIsland
    .contentMargins(.trailing, 8, for:.expanded)
    .contentMargins(.all, 20, for:.expanded)
```

## See Also

### Specifying content margins

struct DynamicIslandMode

A structure that offers values that describe the content mode for a Live Activity.

