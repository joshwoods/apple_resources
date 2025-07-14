

- SpriteKit
- SKView
-  allowsTransparency 

Instance Property

# allowsTransparency

A Boolean property that indicates whether the view is rendered using transparency.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allowsTransparency: Bool { get set }
```

## Mentioned in 

Creating a Scene with a Transparent Background

## Discussion

This property tells the drawing system as to how it should treat the view. If set to false, the drawing system treats the view as fully opaque, which allows the drawing system to optimize some drawing operations and improve performance. If set to true, the drawing system composites the view normally with other content. The default value of this property is false.

An opaque view is expected to fill its bounds with entirely opaque content—that is, the content should have an alpha value of 1.0. If the view is opaque and either does not fill its bounds or contains wholly or partially transparent content, the results are unpredictable. Always set the value of this property to false if the view is fully or partially transparent.

## See Also

### Configuring Performance Related Toggles

var ignoresSiblingOrder: Bool

A Boolean value that indicates whether parent-child and sibling relationships affect the rendering order of nodes in the scene.

var shouldCullNonVisibleNodes: Bool

A Boolean value that indicates whether the view automatically culls non-visible nodes from the rendering tree.

var isAsynchronous: Bool

A Boolean value that indicates whether the content is rendered asynchronously.

