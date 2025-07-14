

- XcodeKit
-  XCSourceTextBuffer 

Class

# XCSourceTextBuffer

A buffer you use to access and modify the text contents and text selections in a source editor.

macOS 10.12+

``` source
class XCSourceTextBuffer
```

## Overview

Mutations to the buffer are tracked and committed when a command completes successfully and has not been canceled by the user.

## Topics

### Accessing Source Text

var completeBuffer: String

The complete buffer’s string representation.

var contentUTI: String

The Uniform Type Identifier (UTI) of the content in the buffer.

### Editing Source Text

var lines: NSMutableArray

The lines of text in the buffer, including line endings.

var selections: NSMutableArray

The text selections in the buffer.

### Configuring Source Editor Indentation

var indentationWidth: Int

The number of space characters used for indentation of the text in the buffer.

var usesTabsForIndentation: Bool

A Boolean value that indicates whether tabs are used for indentation.

var tabWidth: Int

The number of space characters represented by a tab character in the buffer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Source Text

struct XCSourceTextPosition

A zero-based position in a source editor, defined by a line number and column number.

class XCSourceTextRange

A half-open range of text in a buffer you use to select text or specify the insertion point for new text.

