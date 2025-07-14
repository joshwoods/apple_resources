

- BrowserEngineKit
- BETextInput
-  setAttributedMarkedText(\_:selectedRange:) 

Instance Method

# setAttributedMarkedText(\_:selectedRange:)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func setAttributedMarkedText(
    _ markedText: NSAttributedString?,
    selectedRange: NSRange
)
```

**Required**

## See Also

### Marking text

var markedText: String?

String for the text that has been marked as part of an active input session

**Required**

var attributedMarkedText: NSAttributedString?

Attributed string for the text that has been marked as part of an active input session

**Required**

var markedTextRange: UITextRange?

Range representing the position of the markedText.

**Required**

var hasMarkedText: Bool

Indicates whether there any text is currently marked as part of an active input session

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func unmarkText()

Unmarks the currently marked text

**Required**

func isPointNearMarkedText(CGPoint) -> Bool

Returns whether a point should be considered “near” the marked text. Used to determine whether text interaction gestures near marked text should begin.

**Required**

