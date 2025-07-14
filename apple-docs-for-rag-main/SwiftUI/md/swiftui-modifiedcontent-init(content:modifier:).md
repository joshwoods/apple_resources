

- SwiftUI
- ModifiedContent
-  init(content:modifier:) 

Initializer

# init(content:modifier:)

A structure that the defines the content and modifier needed to produce a new view or view modifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    content: Content,
    modifier: Modifier
)
```

## Parameters 

`content`  

The content that the modifier changes.

`modifier`  

The modifier to apply to the content.

## Discussion

If `content` is a View and `modifier` is a ViewModifier, the result is a View. If `content` and `modifier` are both view modifiers, then the result is a new ViewModifier combining them.

## See Also

### Creating a modified content view

var content: Content

The content that the modifier transforms into a new view or new view modifier.

var modifier: Modifier

The view modifier.

