

- InputMethodKit
- IMKInputController
-  candidateSelectionChanged(\_:) 

Instance Method

# candidateSelectionChanged(\_:)

Informs an input controller that the current candidate selection in the candidate window has changed.

macOS 10.5+

``` source
func candidateSelectionChanged(_ candidateString: NSAttributedString!)
```

## Parameters 

`candidateString`  

The changed candidate string.

## Discussion

Note this method is called to indicate user activity in the candidate window. The candidate object might not be the user’s final selection.

## See Also

### Tracking Selections

func annotationSelected(NSAttributedString!, forCandidate: NSAttributedString!)

Sends the selected candidate string and annotation string to the input controller.

func candidateSelected(NSAttributedString!)

Informs an input controller that a new candidate is selected.

