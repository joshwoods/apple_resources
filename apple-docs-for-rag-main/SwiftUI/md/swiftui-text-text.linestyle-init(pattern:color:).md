

- SwiftUI
- Text
- Text.LineStyle
-  init(pattern:color:) 

Initializer

# init(pattern:color:)

Creates a line style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    pattern: Text.LineStyle.Pattern = .solid,
    color: Color? = nil
)
```

## Parameters 

`pattern`  

The pattern of the line.

`color`  

The color of the line. If not provided, the foreground color of text is used.

## See Also

### Creating a text line style

init?(nsUnderlineStyle: NSUnderlineStyle)

Creates a `Text.LineStyle` from `NSUnderlineStyle`.

struct Pattern

The pattern, that the line has.

