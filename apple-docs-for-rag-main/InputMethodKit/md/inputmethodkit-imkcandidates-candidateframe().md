

- InputMethodKit
- IMKCandidates
-  candidateFrame() 

Instance Method

# candidateFrame()

macOS 10.5+

``` source
@MainActor
func candidateFrame() -> NSRect
```

## See Also

### Instance Methods

func attachChild(IMKCandidates!, toCandidate: Int, type: IMKStyleType)

func candidateIdentifier(atLineNumber: Int) -> Int

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

