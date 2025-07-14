

- AppKit
- NSTextFinder
-  isIncrementalSearchingEnabled 

Instance Property

# isIncrementalSearchingEnabled

Determines if incremental searching is enabled.

macOS 10.7+

``` source
var isIncrementalSearchingEnabled: Bool { get set }
```

## Discussion

If true, then the find bar will do incremental searches. If it returns false, then the find bar will behave regularly.

The default value is false.

## See Also

### Incremental Search Configuration

class func drawIncrementalMatchHighlight(in: NSRect)

Override this method to draw custom highlighting.

var incrementalMatchRanges: [NSValue]

Array of incremental search matches posted on the main queue, which have been found during a background search.

var incrementalSearchingShouldDimContentView: Bool

Determines the type of incremental search feedback to be presented

