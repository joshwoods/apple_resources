

- AppKit
- NSTextCheckingController
-  insertedText(in:) 

Instance Method

# insertedText(in:)

macOS 10.15+

``` source
func insertedText(in range: NSRange)
```

## See Also

### Instance Methods

func changeSpelling(Any?)

func checkSpelling(Any?)

func checkText(in: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any])

func checkTextInDocument(Any?)

func checkTextInSelection(Any?)

func considerTextChecking(for: NSRange)

func didChangeSelectedRange()

func didChangeText(in: NSRange)

func ignoreSpelling(Any?)

func invalidate()

func menu(at: Int, clickedOnSelection: Bool, effectiveRange: NSRangePointer) -> NSMenu?

func orderFrontSubstitutionsPanel(Any?)

func showGuessPanel(Any?)

func updateCandidates()

func validAnnotations() -> [NSAttributedString.Key]

