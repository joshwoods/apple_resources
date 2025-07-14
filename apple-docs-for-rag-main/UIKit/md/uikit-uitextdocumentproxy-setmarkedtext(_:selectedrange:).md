

- UIKit
- UITextDocumentProxy
-  setMarkedText(\_:selectedRange:) 

Instance Method

# setMarkedText(\_:selectedRange:)

Inserts the provided text and marks it to indicate that it’s part of an active input session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setMarkedText(
    _ markedText: String,
    selectedRange: NSRange
)
```

**Required**

## Mentioned in 

Handling text interactions in custom keyboards

## Discussion

Setting marked text either replaces the existing marked text or, if none is present, inserts it in place of the current selection.

## See Also

### Managing marked text

func unmarkText()

Unmarks the currently marked text.

**Required**

