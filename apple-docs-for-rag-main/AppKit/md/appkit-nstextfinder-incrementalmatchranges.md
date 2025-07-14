

- AppKit
- NSTextFinder
-  incrementalMatchRanges 

Instance Property

# incrementalMatchRanges

Array of incremental search matches posted on the main queue, which have been found during a background search.

macOS 10.7+

``` source
var incrementalMatchRanges: [NSValue] { get }
```

## Discussion

This array is updated periodically on the main queue as the incremental search operation on a background queue finds matches. You can use this property when incrementalSearchingShouldDimContentView is false to know where to draw highlights for incremental matches.

If no incremental search is active, or there are no matches found, this array will be empty. If an incremental search is currently in progress, but not yet complete, this will return all the ranges found so far.

This array is key-value observing compliant and can be observed to know when to update your highlights. When new and old options are used, the key-value observing change dictionary provides the ranges (and their indexes) that are added or removed. This allows the invalidation of the minimal region necessary to sync highlights with the receiver’s results.

## See Also

### Incremental Search Configuration

class func drawIncrementalMatchHighlight(in: NSRect)

Override this method to draw custom highlighting.

var isIncrementalSearchingEnabled: Bool

Determines if incremental searching is enabled.

var incrementalSearchingShouldDimContentView: Bool

Determines the type of incremental search feedback to be presented

