

- BrowserEngineKit
- BETextDocumentContext
-  autocorrectedRanges 

Instance Property

# autocorrectedRanges

Array of `NSRange` values, relative to the full context string made by combining the `contextBefore`, `markedText` (or `selectedText` if the marked text is empty), and the `contextAfter`.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var autocorrectedRanges: [NSValue] { get set }
```

