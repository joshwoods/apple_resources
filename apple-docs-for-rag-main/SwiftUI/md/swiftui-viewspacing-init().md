

- SwiftUI
- ViewSpacing
-  init() 

Initializer

# init()

Initializes an instance with default spacing values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init()
```

## Discussion

Use this initializer to create a spacing preferences instance with default values. Then use formUnion(_:edges:) to combine preferences from other views with the new instance. You typically do this in a custom layout’s implementation of the spacing(subviews:cache:) method.

## See Also

### Creating spacing instances

static let zero: ViewSpacing

A view spacing instance that contains zero on all edges.

