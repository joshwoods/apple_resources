

- XcodeKit
-  XCSourceTextRange 

Class

# XCSourceTextRange

A half-open range of text in a buffer you use to select text or specify the insertion point for new text.

macOS 10.12+

``` source
class XCSourceTextRange
```

## Overview

Source text ranges are half-open ranges. As a result, source text ranges include the character at the start position but exclude the character at the end position.

A range with equal start and end positions may be used to indicate a point within the buffer, such as an insertion point. The `start` and `end` position may be improperly ordered while you prepare them in your own code, but must be properly ordered before passing an `XCSourceTextRange` instance to other methods.

## Topics

### Creating Source Text Ranges

init(start: XCSourceTextPosition, end: XCSourceTextPosition)

Creates a new source text range defined by its starting and ending positions.

### Getting the Bounds of Source Text Ranges

var start: XCSourceTextPosition

The start position of the range.

var end: XCSourceTextPosition

The end position of the range.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Source Text

class XCSourceTextBuffer

A buffer you use to access and modify the text contents and text selections in a source editor.

struct XCSourceTextPosition

A zero-based position in a source editor, defined by a line number and column number.

