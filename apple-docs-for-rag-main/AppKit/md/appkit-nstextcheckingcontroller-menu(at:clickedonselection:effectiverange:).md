

- AppKit
- NSTextCheckingController
-  menu(at:clickedOnSelection:effectiveRange:) 

Instance Method

# menu(at:clickedOnSelection:effectiveRange:)

macOS 10.15+

``` source
func menu(
    at location: Int,
    clickedOnSelection: Bool,
    effectiveRange: NSRangePointer
) -> NSMenu?
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

func insertedText(in: NSRange)

func invalidate()

func orderFrontSubstitutionsPanel(Any?)

func showGuessPanel(Any?)

func updateCandidates()

func validAnnotations() -> [NSAttributedString.Key]

