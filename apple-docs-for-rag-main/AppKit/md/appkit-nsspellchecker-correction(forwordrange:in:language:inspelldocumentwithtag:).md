

- AppKit
- NSSpellChecker
-  correction(forWordRange:in:language:inSpellDocumentWithTag:) 

Instance Method

# correction(forWordRange:in:language:inSpellDocumentWithTag:)

Returns a single proposed correction if a word is mis-spelled.

macOS 10.7+

``` source
func correction(
    forWordRange range: NSRange,
    in string: String,
    language: String,
    inSpellDocumentWithTag tag: Int
) -> String?
```

## Parameters 

`range`  

The range of the word to be corrected.

`string`  

The string containing the proposed correction.

`language`  

The language.

`tag`  

An identifier unique within the application used to inform the spell checker which document that text is associated, potentially for many purposes, not necessarily just for ignored words. A value of 0 can be passed in for text not associated with a particular document.

## Return Value

The proposed correct string.

## Discussion

While correction functionality is available starting in OS X v10.6 as part of unified text checking, for convenience this method makes it available separately starting in OS X v10.7.

## See Also

### Automatic Spelling Correction

func showCorrectionIndicator(of: NSSpellChecker.CorrectionIndicatorType, primaryString: String, alternativeStrings: [String], forStringIn: NSRect, view: NSView, completionHandler: ((String?) -> Void)?)

Display a suitable user interface to indicate a correction may need to be made.

func record(NSSpellChecker.CorrectionResponse, toCorrection: String, forWord: String, language: String?, inSpellDocumentWithTag: Int)

Records the user response to the correction indicator being displayed.

func dismissCorrectionIndicator(for: NSView)

Dismisses the correction indicator for the specified view.

enum CorrectionIndicatorType

Constants that allow an app to specify the correction indicator type displayed.

enum CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

