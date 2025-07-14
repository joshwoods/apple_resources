

- SwiftUI
- Text
- Text.LineStyle
-  init(nsUnderlineStyle:) 

Initializer

# init(nsUnderlineStyle:)

Creates a `Text.LineStyle` from `NSUnderlineStyle`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(nsUnderlineStyle: NSUnderlineStyle)
```

## Parameters 

`nsUnderlineStyle`  

A value of `NSUnderlineStyle` to wrap with `Text.LineStyle`.

## Return Value

A new `Text.LineStyle` or `nil` when `nsUnderlineStyle` contains styles not supported by `Text.LineStyle`.

## Discussion

Note

Use this initializer only if you need to convert an existing `NSUnderlineStyle` to a SwiftUI `Text.LineStyle`. Otherwise, create a `Text.LineStyle` using an initializer like init(pattern:color:).

## See Also

### Creating a text line style

init(pattern: Text.LineStyle.Pattern, color: Color?)

Creates a line style.

struct Pattern

The pattern, that the line has.

