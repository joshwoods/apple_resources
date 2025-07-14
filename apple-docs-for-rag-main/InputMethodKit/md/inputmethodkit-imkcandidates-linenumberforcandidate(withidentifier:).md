

- InputMethodKit
- IMKCandidates
-  lineNumberForCandidate(withIdentifier:) 

Instance Method

# lineNumberForCandidate(withIdentifier:)

macOS 10.7+

``` source
@MainActor
func lineNumberForCandidate(withIdentifier candidateIdentifier: Int) -> Int
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

func selectCandidate(Int)

func selectCandidate(withIdentifier: Int) -> Bool

func selectedCandidate() -> Int

func selectedCandidateString() -> NSAttributedString!

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

func showChild()

