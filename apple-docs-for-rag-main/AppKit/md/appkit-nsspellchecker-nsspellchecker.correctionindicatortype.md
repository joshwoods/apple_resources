

- AppKit
- NSSpellChecker
-  NSSpellChecker.CorrectionIndicatorType 

Enumeration

# NSSpellChecker.CorrectionIndicatorType

Constants that allow an app to specify the correction indicator type displayed.

macOS

``` source
enum CorrectionIndicatorType
```

## Topics

### Constants

case `default`

The default indicator that shows a proposed correction.

case reversion

Provides the option to revert to the original form after a correction has been made.

case guesses

Shows multiple alternatives from which the user may choose the appropriate spelling.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Automatic Spelling Correction

func correction(forWordRange: NSRange, in: String, language: String, inSpellDocumentWithTag: Int) -> String?

Returns a single proposed correction if a word is mis-spelled.

func showCorrectionIndicator(of: NSSpellChecker.CorrectionIndicatorType, primaryString: String, alternativeStrings: [String], forStringIn: NSRect, view: NSView, completionHandler: ((String?) -> Void)?)

Display a suitable user interface to indicate a correction may need to be made.

func record(NSSpellChecker.CorrectionResponse, toCorrection: String, forWord: String, language: String?, inSpellDocumentWithTag: Int)

Records the user response to the correction indicator being displayed.

func dismissCorrectionIndicator(for: NSView)

Dismisses the correction indicator for the specified view.

enum CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

