

- InputMethodKit
- IMKCandidates
-  selectedCandidateString() 

Instance Method

# selectedCandidateString()

macOS 10.7+

``` source
@MainActor
func selectedCandidateString() -> NSAttributedString!
```

## See Also

### Instance Methods

func attachChild(IMKCandidates!, toCandidate: Int, type: IMKStyleType)

func candidateFrame() -> NSRect

func candidateIdentifier(atLineNumber: Int) -> Int

func candidateStringIdentifier(Any!) -> Int

func clearSelection()

func detachChild(Int)

func hideChild()

func lineNumberForCandidate(withIdentifier: Int) -> Int

func selectCandidate(Int)

func selectCandidate(withIdentifier: Int) -> Bool

func selectedCandidate() -> Int

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

func showChild()

