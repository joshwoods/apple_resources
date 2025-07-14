

- UIKit
- UITextInput
-  beginningOfDocument 

Instance Property

# beginningOfDocument

The text position for the beginning of a document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var beginningOfDocument: UITextPosition { get }
```

**Required**

## See Also

### Computing text ranges and text positions

func textRange(from: UITextPosition, to: UITextPosition) -> UITextRange?

Returns the range between two text positions.

**Required**

func position(from: UITextPosition, offset: Int) -> UITextPosition?

Returns the text position at a specified offset from another text position.

**Required**

func position(from: UITextPosition, in: UITextLayoutDirection, offset: Int) -> UITextPosition?

Returns the text position at a specified offset in a specified direction from another text position.

**Required**

var endOfDocument: UITextPosition

The text position for the end of a document.

**Required**

