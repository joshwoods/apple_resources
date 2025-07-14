

- BrowserEngineKit
- BETextInput
-  markedTextRange 

Instance Property

# markedTextRange

Range representing the position of the markedText.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var markedTextRange: UITextRange? { get }
```

**Required**

## Discussion

If text can be selected, it can be marked. Marked text represents provisionally inserted text that has yet to be confirmed by the user. It requires unique visual treatment in its display. If there is any marked text, the selection, whether a caret or an extended range, always resides within.

Setting marked text either replaces the existing marked text or, if none is present, inserts it from the current selection.

Return nil if no marked text

## See Also

### Marking text

var markedText: String?

String for the text that has been marked as part of an active input session

**Required**

var attributedMarkedText: NSAttributedString?

Attributed string for the text that has been marked as part of an active input session

**Required**

var hasMarkedText: Bool

Indicates whether there any text is currently marked as part of an active input session

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

**Required**

func unmarkText()

Unmarks the currently marked text

**Required**

func isPointNearMarkedText(CGPoint) -> Bool

Returns whether a point should be considered “near” the marked text. Used to determine whether text interaction gestures near marked text should begin.

**Required**

