

- AppKit
-  NSTextCheckingController 

Class

# NSTextCheckingController

macOS 10.15+

``` source
class NSTextCheckingController
```

## Topics

### Initializers

init(client: any NSTextCheckingClient)

### Instance Properties

var client: any NSTextCheckingClient

var spellCheckerDocumentTag: Int

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

func menu(at: Int, clickedOnSelection: Bool, effectiveRange: NSRangePointer) -> NSMenu?

func orderFrontSubstitutionsPanel(Any?)

func showGuessPanel(Any?)

func updateCandidates()

func validAnnotations() -> [NSAttributedString.Key]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Text-checking

protocol NSTextCheckingClient

protocol NSTextInputTraits

enum NSTextInputTraitType

