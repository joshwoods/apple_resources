

- SwiftUI
-  TextProxy 

Structure

# TextProxy

A proxy for a text view that custom text renderers use.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TextProxy
```

## Topics

### Instance Methods

func sizeThatFits(ProposedViewSize) -> CGSize

Returns the space needed by the text view, for a proposed size.

## See Also

### Rendering text

Creating visual effects with SwiftUI

Add scroll effects, rich color treatments, custom transitions, and advanced effects using shaders and a text renderer.

protocol TextAttribute

A value that you can attach to text views and that text renderers can query.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

protocol TextRenderer

A value that can replace the default text view rendering behavior.

