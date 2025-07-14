

- AppKit
- NSTextCheckingController
-  checkText(in:types:options:) 

Instance Method

# checkText(in:types:options:)

macOS 10.15+

``` source
func checkText(
    in range: NSRange,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any] = [:]
)
```

## See Also

### Instance Methods

func changeSpelling(Any?)

func checkSpelling(Any?)

func checkTextInDocument(Any?)

func checkTextInSelection(Any?)

func considerTextChecking(for: NSRange)

func didChangeSelectedRange()

func didChangeText(in: NSRange)

func ignoreSpelling(Any?)

func insertedText(in: NSRange)

func invalidate()

func menu(at: Int, clickedOnSelection: Bool, effectiveRange: NSRangePointer) -> NSMenu?

func orderFrontSubstitutionsPanel(Any?)

func showGuessPanel(Any?)

func updateCandidates()

func validAnnotations() -> [NSAttributedString.Key]

