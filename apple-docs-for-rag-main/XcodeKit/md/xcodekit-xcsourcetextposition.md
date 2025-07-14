

- XcodeKit
-  XCSourceTextPosition 

Structure

# XCSourceTextPosition

A zero-based position in a source editor, defined by a line number and column number.

macOS 10.12+

``` source
struct XCSourceTextPosition
```

## Topics

### Creating Source Text Positions

init()

Creates a new source text position at the beginning of the source text.

init(line: Int, column: Int)

Creates a source text position at the specified line and column.

### Inspecting Source Text Positions

var column: Int

The horizontal component of a source text position.

var line: Int

The vertical component of a source text position.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Source Text

class XCSourceTextBuffer

A buffer you use to access and modify the text contents and text selections in a source editor.

class XCSourceTextRange

A half-open range of text in a buffer you use to select text or specify the insertion point for new text.

