

- InputMethodKit
- IMKCandidates
-  selectCandidate(withIdentifier:) 

Instance Method

# selectCandidate(withIdentifier:)

macOS 10.7+

``` source
@MainActor
func selectCandidate(withIdentifier candidateIdentifier: Int) -> Bool
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

func selectedCandidate() -> Int

func selectedCandidateString() -> NSAttributedString!

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

func showChild()

