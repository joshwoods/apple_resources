

- BrowserEngineKit
- BEResponderEditActions
-  transliterateChinese(\_:) 

Instance Method

# transliterateChinese(\_:)

Converts the selected text between traditional and simplified Chinese.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
optional func transliterateChinese(_ sender: Any?)
```

## Overview

To invoke the standard operating system behavior for transliterating Chinese text, call transliterateChinese(forText:) in your implementation of this method.

When you change the selected text in your implementation of this method, notify the operating system by calling selectionWillChange(for:) and selectionDidChange(for:).

## See Also

### Translating and transliterating text

func translate(Any?)

Presents a translation of the selected text.

