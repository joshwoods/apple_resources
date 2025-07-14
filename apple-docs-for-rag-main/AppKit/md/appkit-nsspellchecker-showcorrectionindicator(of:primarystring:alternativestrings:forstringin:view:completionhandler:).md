

- AppKit
- NSSpellChecker
-  showCorrectionIndicator(of:primaryString:alternativeStrings:forStringIn:view:completionHandler:) 

Instance Method

# showCorrectionIndicator(of:primaryString:alternativeStrings:forStringIn:view:completionHandler:)

Display a suitable user interface to indicate a correction may need to be made.

macOS 10.7+

``` source
func showCorrectionIndicator(
    of type: NSSpellChecker.CorrectionIndicatorType,
    primaryString: String,
    alternativeStrings: [String],
    forStringIn rectOfTypedString: NSRect,
    view: NSView,
    completionHandler completionBlock: ((String?) -> Void)? = nil
)
```

``` source
func showCorrectionIndicator(
    of type: NSSpellChecker.CorrectionIndicatorType,
    primaryString: String,
    alternativeStrings: [String],
    forStringIn rectOfTypedString: NSRect,
    view: NSView
) async -> String?
```

## Parameters 

`type`  

The correction type to display. See NSSpellChecker.CorrectionIndicatorType for possible values.

`primaryString`  

The first string to be displayed, a correction or reversion according to the `type` of indicator.

`alternativeStrings`  

An array of alternative strings to insert. This array may be empty.

`rectOfTypedString`  

The rectangle of the typed text.

`view`  

The view in which the correction indicator is to be displayed.

`completionBlock`  

The Block called when a the correction indicator is dismissed.

The Block takes one argument:

acceptedString  
The correction string the user excepted. If the user does not select a correction string nil is returned.

## Discussion

Only one indicator at a time may be displayed for a given view, and the only thing a client may do with the indicator after displaying it is to dismiss it using the dismissCorrectionIndicator(for:) method.

Note

In order to record responses properly (for use with the record(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method), clients must store the original word and original correction at least from the point at which the user accepts it until the user edits or reverts it.

## See Also

### Automatic Spelling Correction

func correction(forWordRange: NSRange, in: String, language: String, inSpellDocumentWithTag: Int) -> String?

Returns a single proposed correction if a word is mis-spelled.

func record(NSSpellChecker.CorrectionResponse, toCorrection: String, forWord: String, language: String?, inSpellDocumentWithTag: Int)

Records the user response to the correction indicator being displayed.

func dismissCorrectionIndicator(for: NSView)

Dismisses the correction indicator for the specified view.

enum CorrectionIndicatorType

Constants that allow an app to specify the correction indicator type displayed.

enum CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

