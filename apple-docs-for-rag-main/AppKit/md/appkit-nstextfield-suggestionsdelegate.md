

- AppKit
- NSTextField
-  suggestionsDelegate 

Instance Property

# suggestionsDelegate

The delegate that provides text suggestions for the receiving text field and responds to the user highlighting and selecting items.

macOS 15.0+

``` source
@MainActor @preconcurrency
weak var suggestionsDelegate: (any NSTextSuggestionsDelegate)? { get set }
```

