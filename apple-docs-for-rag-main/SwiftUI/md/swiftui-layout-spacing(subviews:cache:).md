

- SwiftUI
- Layout
-  spacing(subviews:cache:) 

Instance Method

# spacing(subviews:cache:)

Returns the preferred spacing values of the composite view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func spacing(
    subviews: Self.Subviews,
    cache: inout Self.Cache
) -> ViewSpacing
```

**Required** Default implementation provided.

## Parameters 

`subviews`  

A collection of proxy instances that represent the views that the container arranges. You can use the proxies in the collection to get information about the subviews as you determine how much spacing the container prefers around it.

`cache`  

Optional storage for calculated data that you can share among the methods of your custom layout container. See makeCache(subviews:) for details.

## Return Value

A ViewSpacing instance that describes the preferred spacing around the container view.

## Discussion

Implement this method to provide custom spacing preferences for a layout container. The value you return affects the spacing around the container, but it doesn’t affect how the container arranges subviews relative to one another inside the container.

Create a custom ViewSpacing instance for your container by initializing one with default values, and then merging that with spacing instances of certain subviews. For example, if you define a basic vertical stack that places subviews in a column, you could use the spacing preferences of the subview edges that make contact with the container’s edges:

```
extension BasicVStack {
    func spacing(subviews: Subviews, cache: inout ()) -> ViewSpacing {
        var spacing = ViewSpacing()

        for index in subviews.indices {
            var edges: Edge.Set = [.leading, .trailing]
            if index == 0 { edges.formUnion(.top) }
            if index == subviews.count - 1 { edges.formUnion(.bottom) }
            spacing.formUnion(subviews[index].spacing, edges: edges)
        }

        return spacing
    }
}
```

In the above example, the first and last subviews contribute to the spacing above and below the container, respectively, while all subviews affect the spacing on the leading and trailing edges.

If you don’t implement this method, the protocol provides a default implementation that merges the spacing preferences across all subviews on all edges.

## Default Implementations

### Layout Implementations

func spacing(subviews: Self.Subviews, cache: inout Self.Cache) -> ViewSpacing

Returns the union of all subview spacing.

## See Also

### Reporting layout container characteristics

func explicitAlignment(of:in:proposal:subviews:cache:)

Returns the position of the specified horizontal alignment guide along the x axis.

**Required** Default implementations provided.

static var layoutProperties: LayoutProperties

Properties of a layout container.

**Required** Default implementation provided.

