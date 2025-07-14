

- InputMethodKit
- IMKInputController
-  annotationSelected(\_:forCandidate:) 

Instance Method

# annotationSelected(\_:forCandidate:)

Sends the selected candidate string and annotation string to the input controller.

macOS 10.5+

``` source
func annotationSelected(
    _ annotationString: NSAttributedString!,
    forCandidate candidateString: NSAttributedString!
)
```

## Parameters 

`annotationString`  

The annotation string associated with the candidate.

`candidateString`  

The candidate string that the user moved to.

## Discussion

This method is called when the user moves to a candidate.

## See Also

### Tracking Selections

func candidateSelectionChanged(NSAttributedString!)

Informs an input controller that the current candidate selection in the candidate window has changed.

func candidateSelected(NSAttributedString!)

Informs an input controller that a new candidate is selected.

