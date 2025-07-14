

- InputMethodKit
- IMKCandidates
-  showSublist(\_:subListDelegate:) 

Instance Method

# showSublist(\_:subListDelegate:)

macOS 10.5+

``` source
@MainActor
func showSublist(
    _ candidates: [Any]!,
    subListDelegate delegate: Any!
)
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

func selectedCandidateString() -> NSAttributedString!

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

