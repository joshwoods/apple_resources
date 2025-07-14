

- InputMethodKit
- IMKInputController
-  candidateSelected(\_:) 

Instance Method

# candidateSelected(\_:)

Informs an input controller that a new candidate is selected.

macOS 10.5+

``` source
func candidateSelected(_ candidateString: NSAttributedString!)
```

## Parameters 

`candidateString`  

The changed candidate string.

## Discussion

The candidate object is the user’s final choice from the candidate window. The candidate window is closed before this method is called.

## See Also

### Tracking Selections

func annotationSelected(NSAttributedString!, forCandidate: NSAttributedString!)

Sends the selected candidate string and annotation string to the input controller.

func candidateSelectionChanged(NSAttributedString!)

Informs an input controller that the current candidate selection in the candidate window has changed.

