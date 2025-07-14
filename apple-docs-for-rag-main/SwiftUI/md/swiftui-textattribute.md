

- SwiftUI
-  TextAttribute 

Protocol

# TextAttribute

A value that you can attach to text views and that text renderers can query.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol TextAttribute : Hashable
```

## Relationships

### Inherits From

- Equatable
- Hashable

## See Also

### Rendering text

Creating visual effects with SwiftUI

Add scroll effects, rich color treatments, custom transitions, and advanced effects using shaders and a text renderer.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

protocol TextRenderer

A value that can replace the default text view rendering behavior.

struct TextProxy

A proxy for a text view that custom text renderers use.

