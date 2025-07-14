

- SwiftUI
-  TextRenderer 

Protocol

# TextRenderer

A value that can replace the default text view rendering behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol TextRenderer : Animatable
```

## Topics

### Instance Properties

var displayPadding: EdgeInsets

Returns the size of the extra padding added to any drawing layer used to rasterize the text. For example when drawing the text with a shadow this may be used to extend the drawing bounds to avoid clipping the shadow.

**Required** Default implementation provided.

### Instance Methods

func draw(layout: Text.Layout, in: inout GraphicsContext)

Draws `layout` into `ctx`.

**Required**

func sizeThatFits(proposal: ProposedViewSize, text: TextProxy) -> CGSize

Returns the size of the text in `proposal`. The provided `text` proxy value may be used to query the sizing behavior of the underlying text layout.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Animatable

## See Also

### Rendering text

Creating visual effects with SwiftUI

Add scroll effects, rich color treatments, custom transitions, and advanced effects using shaders and a text renderer.

protocol TextAttribute

A value that you can attach to text views and that text renderers can query.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

struct TextProxy

A proxy for a text view that custom text renderers use.

