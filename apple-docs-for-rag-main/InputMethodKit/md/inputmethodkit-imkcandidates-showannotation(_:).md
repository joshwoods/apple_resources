

- InputMethodKit
- IMKCandidates
-  showAnnotation(\_:) 

Instance Method

# showAnnotation(\_:)

Displays an annotation string in an annotation window.

macOS 10.5+

``` source
@MainActor
func showAnnotation(_ annotationString: NSAttributedString!)
```

## Parameters 

`annotationString`  

The string to display.

## Discussion

An annotation string explains or comments on the candidate string in the candidates window. An annotation window is a small, borderless window that is aligned with the current candidates window. An input method calls `showAnnotation:` when the `candidateSelectionChanged:` method of the IMKInputController class is called, and the candidate string has annotations.

