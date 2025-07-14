

- XcodeKit
- XCSourceTextBuffer
-  lines 

Instance Property

# lines

The lines of text in the buffer, including line endings.

macOS 10.12+

``` source
var lines: NSMutableArray { get }
```

## Discussion

Line breaks within a single buffer should be consistent. Adding a line containing additional line breaks modifies the array such that each line added is a separate element. Changes to the `completeBuffer` property are immediately reflected in this property, and vice versa.

## See Also

### Editing Source Text

var selections: NSMutableArray

The text selections in the buffer.

