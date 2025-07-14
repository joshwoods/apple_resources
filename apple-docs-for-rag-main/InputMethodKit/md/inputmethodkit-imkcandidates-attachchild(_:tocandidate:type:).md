

- InputMethodKit
- IMKCandidates
-  attachChild(\_:toCandidate:type:) 

Instance Method

# attachChild(\_:toCandidate:type:)

macOS 10.7+

``` source
@MainActor
func attachChild(
    _ child: IMKCandidates!,
    toCandidate candidateIdentifier: Int,
    type theType: IMKStyleType
)
```

## See Also

### Instance Methods

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

func showChild()

