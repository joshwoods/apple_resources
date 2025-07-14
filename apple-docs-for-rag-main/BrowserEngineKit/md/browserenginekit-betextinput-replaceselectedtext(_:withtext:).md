

- BrowserEngineKit
- BETextInput
-  replaceSelectedText(\_:withText:) 

Instance Method

# replaceSelectedText(\_:withText:)

Replaces the specified `text` with `replacementText`

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func replaceSelectedText(
    _ text: String,
    withText replacementText: String
)
```

**Required**

## Parameters 

`text`  

The text to replace.

`replacementText`  

The new text to use as the replacement.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

1.  If there is a nonzero length current selection, then replace text with replacementText.

2.  If there is zero length current selection, then replace the matching word before the selection

3.  If the zero length selection is at the start of the element, then replace the matching word after the selection

Replaces the specified text with another string.

## Overview

Your implementation of this method needs to vary its behavior based on the current text selection.

- If the selection has `0` length and is at the start of the document, replace the matching word after the selection.

- If the selection has `0` length and is anywhere else in the document, replace the matching word before the selection.

- Otherwise, replace the selected text.

## See Also

### Replacing text

var isReplaceAllowed: Bool

Returns whether replacement should be allowed for an editable element.

**Required**

