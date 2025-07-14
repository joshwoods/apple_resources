

- SwiftUI
- Text
-  textScale(\_:isEnabled:) 

Instance Method

# textScale(\_:isEnabled:)

Applies a text scale to the text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func textScale(
    _ scale: Text.Scale,
    isEnabled: Bool = true
) -> Text
```

## Parameters 

`scale`  

The text scale to apply.

`isEnabled`  

If true the text scale is applied; otherwise text scale is unchanged.

## Return Value

Text with the specified scale applied.

## See Also

### Fitting text into available space

struct Scale

Defines text scales

enum TruncationMode

The type of truncation to apply to a line of text when it’s too long to fit in the available space.

