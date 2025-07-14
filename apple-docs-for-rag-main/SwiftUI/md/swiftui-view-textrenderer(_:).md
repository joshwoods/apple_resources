

- SwiftUI
- View
-  textRenderer(\_:) 

Instance Method

# textRenderer(\_:)

Returns a new view such that any text views within it will use `renderer` to draw themselves.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func textRenderer(_ renderer: T) -> some View where T : TextRenderer
```

## Parameters 

`renderer`  

The renderer value.

## Return Value

A new view that will use `renderer` to draw its text views.

## See Also

### Rendering text

Creating visual effects with SwiftUI

Add scroll effects, rich color treatments, custom transitions, and advanced effects using shaders and a text renderer.

protocol TextAttribute

A value that you can attach to text views and that text renderers can query.

protocol TextRenderer

A value that can replace the default text view rendering behavior.

struct TextProxy

A proxy for a text view that custom text renderers use.

