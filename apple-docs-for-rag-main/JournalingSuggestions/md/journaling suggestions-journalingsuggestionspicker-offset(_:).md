

- Journaling Suggestions
- JournalingSuggestionsPicker
-  offset(\_:) 

Instance Method

# offset(\_:)

Offset this view by the horizontal and vertical amount specified in the offset parameter.

Journaling SuggestionsSwiftUIiOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func offset(_ offset: CGSize) -> some View
```

## Parameters 

`offset`  

The distance to offset this view.

## Return Value

A view that offsets this view by `offset`.

## Discussion

Use `offset(_:)` to shift the displayed contents by the amount specified in the `offset` parameter.

The original dimensions of the view aren’t changed by offsetting the contents; in the example below the gray border drawn by this view surrounds the original position of the text:

```
Text("Offset by passing CGSize()")
    .border(Color.green)
    .offset(CGSize(width: 20, height: 25))
    .border(Color.gray)
```

