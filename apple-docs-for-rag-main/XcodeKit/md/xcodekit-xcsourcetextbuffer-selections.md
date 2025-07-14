

- XcodeKit
- XCSourceTextBuffer
-  selections 

Instance Property

# selections

The text selections in the buffer.

macOS 10.12+

``` source
var selections: NSMutableArray { get }
```

## Discussion

An empty range represents an insertion point. Modifying the lines of text in the buffer automatically updates the selections to match.

## See Also

### Editing Source Text

var lines: NSMutableArray

The lines of text in the buffer, including line endings.

