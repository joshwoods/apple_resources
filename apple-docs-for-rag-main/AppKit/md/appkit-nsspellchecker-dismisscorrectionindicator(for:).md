

- AppKit
- NSSpellChecker
-  dismissCorrectionIndicator(for:) 

Instance Method

# dismissCorrectionIndicator(for:)

Dismisses the correction indicator for the specified view.

macOS 10.7+

``` source
func dismissCorrectionIndicator(for view: NSView)
```

## Parameters 

`view`  

The view.

## See Also

### Automatic Spelling Correction

func correction(forWordRange: NSRange, in: String, language: String, inSpellDocumentWithTag: Int) -> String?

Returns a single proposed correction if a word is mis-spelled.

func showCorrectionIndicator(of: NSSpellChecker.CorrectionIndicatorType, primaryString: String, alternativeStrings: [String], forStringIn: NSRect, view: NSView, completionHandler: ((String?) -> Void)?)

Display a suitable user interface to indicate a correction may need to be made.

func record(NSSpellChecker.CorrectionResponse, toCorrection: String, forWord: String, language: String?, inSpellDocumentWithTag: Int)

Records the user response to the correction indicator being displayed.

enum CorrectionIndicatorType

Constants that allow an app to specify the correction indicator type displayed.

enum CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

