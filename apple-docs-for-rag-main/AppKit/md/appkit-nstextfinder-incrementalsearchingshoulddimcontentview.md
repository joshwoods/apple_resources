

- AppKit
- NSTextFinder
-  incrementalSearchingShouldDimContentView 

Instance Property

# incrementalSearchingShouldDimContentView

Determines the type of incremental search feedback to be presented

macOS 10.7+

``` source
var incrementalSearchingShouldDimContentView: Bool { get set }
```

## Discussion

If true, then when an incremental search begins, the `findBarContainer` instance’s parent `contentView` will be dimmed, except for the locations of the incremental matches. If false, then the incremental matches will not be highlighted automatically, but you can use incrementalMatchRanges to highlight the matches yourself.

The default value is true.

## See Also

### Incremental Search Configuration

class func drawIncrementalMatchHighlight(in: NSRect)

Override this method to draw custom highlighting.

var incrementalMatchRanges: [NSValue]

Array of incremental search matches posted on the main queue, which have been found during a background search.

var isIncrementalSearchingEnabled: Bool

Determines if incremental searching is enabled.

