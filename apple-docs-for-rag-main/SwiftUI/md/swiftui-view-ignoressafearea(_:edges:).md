

- SwiftUI
- View
-  ignoresSafeArea(\_:edges:) 

Instance Method

# ignoresSafeArea(\_:edges:)

Expands the safe area of a view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func ignoresSafeArea(
    _ regions: SafeAreaRegions = .all,
    edges: Edge.Set = .all
) -> some View
```

## Parameters 

`regions`  

The regions to expand the view’s safe area into. The modifier expands into all safe area region types by default.

`edges`  

The set of edges to expand. Any edges that you don’t include in this set remain unchanged. The set includes all edges by default.

## Return Value

A view with an expanded safe area.

## Mentioned in 

Adding a background to your view

## Discussion

By default, the SwiftUI layout system sizes and positions views to avoid certain safe areas. This ensures that system content like the software keyboard or edges of the device don’t obstruct your views. To extend your content into these regions, you can ignore safe areas on specific edges by applying this modifier.

For examples of how to use this modifier, see Adding a background to your view.

## See Also

### Staying in the safe areas

func safeAreaInset(edge:alignment:spacing:content:)

Shows the specified content beside the modified view.

func safeAreaPadding(_:)

Adds the provided insets into the safe area of this view.

func safeAreaPadding(Edge.Set, CGFloat?) -> some View

Adds the provided insets into the safe area of this view.

struct SafeAreaRegions

A set of symbolic safe area regions.

