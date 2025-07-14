

- AppKit
- NSCollectionLayoutContainer
-  contentInsets 

Instance Property

# contentInsets

The amount of space added around the content of the container to adjust its final size.

macOS 10.15+

``` source
@MainActor
var contentInsets: NSDirectionalEdgeInsets { get }
```

**Required**

## Discussion

If the value of a content inset is less than `1.0`, the content inset is fractional. For example, a top content inset of `20.0` adds 20 points of space between the top of the layout and the top of its container. A top content inset of `0.2` adds space equal to 20% of the container’s height between the top of the layout and the top of its container.

## See Also

### Getting content insets

var effectiveContentInsets: NSDirectionalEdgeInsets

The amount of space added around the content of the container to adjust its final size after item content insets are applied.

**Required**

