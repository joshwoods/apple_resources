

- InputMethodKit
- IMKCandidates
-  candidateIdentifier(atLineNumber:) 

Instance Method

# candidateIdentifier(atLineNumber:)

macOS 10.7+

``` source
@MainActor
func candidateIdentifier(atLineNumber lineNumber: Int) -> Int
```

## See Also

### Instance Methods

func attachChild(IMKCandidates!, toCandidate: Int, type: IMKStyleType)

func candidateFrame() -> NSRect

func candidateStringIdentifier(Any!) -> Int

func clearSelection()

func detachChild(Int)

func hideChild()

func lineNumberForCandidate(withIdentifier: Int) -> Int

func selectCandidate(Int)

func selectCandidate(withIdentifier: Int) -> Bool

func selectedCandidate() -> Int

func selectedCandidateString() -> NSAttributedString!

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

func showChild()

