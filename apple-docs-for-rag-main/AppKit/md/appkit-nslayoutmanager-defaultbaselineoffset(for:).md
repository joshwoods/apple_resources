

- AppKit
- NSLayoutManager
-  defaultBaselineOffset(for:) 

Instance Method

# defaultBaselineOffset(for:)

Returns the default baseline offset that the layout manager’s typesetter uses for the specified font.

macOS 10.7+

``` source
func defaultBaselineOffset(for theFont: NSFont) -> CGFloat
```

## Parameters 

`theFont`  

The font for which to return the default baseline offset.

## Return Value

The default baseline offset for a line of text drawn using `theFont`.

## Discussion

The value returned may vary according to the layout manager’s typesetter behavior.

## See Also

### Managing the typesetter

var typesetter: NSTypesetter

The current typesetter.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The default typesetter behavior.

enum TypesetterBehavior

Constants that determine the layout manager’s behavior during layout.

func defaultLineHeight(for: NSFont) -> CGFloat

Returns the default line height for a line of text that uses a specified font.

