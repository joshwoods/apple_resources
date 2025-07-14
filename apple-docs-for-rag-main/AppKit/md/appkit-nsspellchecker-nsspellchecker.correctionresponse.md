

- AppKit
- NSSpellChecker
-  NSSpellChecker.CorrectionResponse 

Enumeration

# NSSpellChecker.CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

macOS

``` source
enum CorrectionResponse
```

## Topics

### Enumeration Cases

case accepted

The user accepted the correction.

case edited

After the correction was accepted, the user edited the corrected word (to something other than its original form.

case ignored

The user continued in such a way as to ignore the correction.

case none

No response was received from the user.

case rejected

The user rejected the correction by dismissing the correction indicator.

case reverted

After the correction was accepted, the user reverted the correction back to the original word.

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

enum CorrectionIndicatorType

Constants that allow an app to specify the correction indicator type displayed.

