

- AppKit
- NSTextFinder
-  drawIncrementalMatchHighlight(in:) 

Type Method

# drawIncrementalMatchHighlight(in:)

Override this method to draw custom highlighting.

macOS 10.7+

``` source
class func drawIncrementalMatchHighlight(in rect: NSRect)
```

## Parameters 

`rect`  

The rectangle that needs to be drawn highlighted in the current coordinate system.

## Discussion

If incrementalSearchingShouldDimContentView is false, it is recommended to highlight incremental matches in your own view. However, some applications may choose to show incremental search values in a different manner.

This method is not recommended to be overridden. The text finder never calls it. The view calls it to get the standard highlight behavior. It is recommended that views use this method do draw the highlight for consistency and to allow Application Kit to tweak the behavior in the future. If the view wants custom drawing, then it should be implemented by the view.

The common usage pattern for this is: draw the background, draw the incremental match highlights for the incrementalMatchRanges, and then draw the text.

## See Also

### Incremental Search Configuration

var incrementalMatchRanges: [NSValue]

Array of incremental search matches posted on the main queue, which have been found during a background search.

var isIncrementalSearchingEnabled: Bool

Determines if incremental searching is enabled.

var incrementalSearchingShouldDimContentView: Bool

Determines the type of incremental search feedback to be presented

