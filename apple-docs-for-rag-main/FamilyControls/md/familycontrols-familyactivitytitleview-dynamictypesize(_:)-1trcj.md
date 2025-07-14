

- FamilyControls
- FamilyActivityTitleView
-  dynamicTypeSize(\_:) 

Instance Method

# dynamicTypeSize(\_:)

Sets the Dynamic Type size within the view to the given value.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func dynamicTypeSize(_ size: DynamicTypeSize) -> some View
```

## Parameters 

`size`  

The size to set for this view.

## Return Value

A view that sets the Dynamic Type size to the specified `size`.

## Discussion

As an example, you can set a Dynamic Type size in `ContentView` to be `DynamicTypeSize/xLarge` (this can be useful in previews to see your content at a different size) like this:

```
ContentView()
    .dynamicTypeSize(.xLarge)
```

If a Dynamic Type size range is applied after setting a value, the value is limited by that range:

```
ContentView() // Dynamic Type size will be .large
    .dynamicTypeSize(...DynamicTypeSize.large)
    .dynamicTypeSize(.xLarge)
```

When limiting the Dynamic Type size, consider if adding a large content view with `View/accessibilityShowsLargeContentViewer()` would be appropriate.

