

- SwiftUI
- Text input and output
-  Creating visual effects with SwiftUI 

Sample Code

# Creating visual effects with SwiftUI

Add scroll effects, rich color treatments, custom transitions, and advanced effects using shaders and a text renderer.

Download

iOS 18.0+iPadOS 18.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC24 session 10151: Create custom visual effects in SwiftUI.

## See Also

### Rendering text

protocol TextAttribute

A value that you can attach to text views and that text renderers can query.

func textRenderer&lt;T>(T) -> some View

Returns a new view such that any text views within it will use `renderer` to draw themselves.

protocol TextRenderer

A value that can replace the default text view rendering behavior.

struct TextProxy

A proxy for a text view that custom text renderers use.

