

- RealityKit
- ObjectCaptureView
-  dynamicTypeSize(\_:) 

Instance Method

# dynamicTypeSize(\_:)

Limits the Dynamic Type size within the view to the given range.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func dynamicTypeSize(_ range: T) -> some View where T : RangeExpression, T.Bound == DynamicTypeSize
```

## Parameters 

`range`  

The range of sizes that are allowed in this view.

## Return Value

A view that constrains the Dynamic Type size of this view within the specified `range`.

## Discussion

As an example, you can constrain the maximum Dynamic Type size in `ContentView` to be no larger than `DynamicTypeSize/large`:

```
ContentView()
    .dynamicTypeSize(...DynamicTypeSize.large)
```

If the Dynamic Type size is limited to multiple ranges, the result is their intersection:

```
ContentView() // Dynamic Type sizes are from .small to .large
    .dynamicTypeSize(.small...)
    .dynamicTypeSize(...DynamicTypeSize.large)
```

A specific Dynamic Type size can still be set after a range is applied:

```
ContentView() // Dynamic Type size is .xLarge
    .dynamicTypeSize(.xLarge)
    .dynamicTypeSize(...DynamicTypeSize.large)
```

When limiting the Dynamic Type size, consider if adding a large content view with `View/accessibilityShowsLargeContentViewer()` would be appropriate.

