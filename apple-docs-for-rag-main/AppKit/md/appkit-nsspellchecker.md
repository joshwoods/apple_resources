

- AppKit
-  NSSpellChecker 

Class

# NSSpellChecker

An interface to the Cocoa spell-checking service.

macOS

``` source
class NSSpellChecker
```

## Overview

To handle all its spell checking, an app needs only one instance of NSSpellChecker, known as the spell checker. Using the spell checker you manage the Spelling panel, in which the user can specify decisions about words that are suspect. The spell checker also offers the ability to provide word completions to augment the text completion system.

## Topics

### Getting the Spell Checker

class var shared: NSSpellChecker

Returns the NSSpellChecker (one per application).

class var sharedSpellCheckerExists: Bool

Returns whether the application’s NSSpellChecker has already been created.

### Configuring Spell Checkers Languages

var availableLanguages: [String]

Provides a list of all available languages.

var userPreferredLanguages: [String]

Provides a subset of the available languages to be used for spell checking.

var automaticallyIdentifiesLanguages: Bool

Sets whether the spell checker will automatically identify languages.

func language() -> String

Returns the current language used in spell checking.

func setLanguage(String) -> Bool

Returns whether the specified language is in the Spelling pop-up list.

### Managing Panels

var spellingPanel: NSPanel

Returns the spell checker’s panel.

var substitutionsPanel: NSPanel

Returns the substitutions panel.

func updateSpellingPanel(withGrammarString: String, detail: [String : Any])

Specifies a grammar-analysis detail to highlight in the Spelling panel.

func updatePanels()

Updates the available panels to account for user changes.

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

### Checking Strings for Spelling and Grammar

func countWords(in: String, language: String?) -> Int

Returns the number of words in the specified string.

func checkSpelling(of: String, startingAt: Int) -> NSRange

Starts the search for a misspelled word in `stringToCheck` starting at `startingOffset` within the string object.

func checkSpelling(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, wordCount: UnsafeMutablePointer&lt;Int>?) -> NSRange

Starts the search for a misspelled word in a string starting at specified offset within the string.

func checkGrammar(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Initiates a grammatical analysis of a given string.

func check(String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, orthography: AutoreleasingUnsafeMutablePointer&lt;NSOrthography?>?, wordCount: UnsafeMutablePointer&lt;Int>?) -> [NSTextCheckingResult]

Requests unified text checking for the given range of the given string.

func requestChecking(of: String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)?) -> Int

Requests that the string be checked in the background.

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

### Managing the Spell-Checking Process

class func uniqueSpellDocumentTag() -> Int

Returns a guaranteed unique tag to use as the spell-document tag for a document.

func closeSpellDocument(withTag: Int)

Notifies the receiver that the user has finished with the tagged document.

func ignoreWord(String, inSpellDocumentWithTag: Int)

Instructs the spell checker to ignore all future occurrences of `wordToIgnore` in the document identified by `tag`.

func ignoredWords(inSpellDocumentWithTag: Int) -> [String]?

Returns the array of ignored words for a document identified by `tag`.

func setIgnoredWords([String], inSpellDocumentWithTag: Int)

Initializes the ignored-words document (a dictionary identified by `tag` with `someWords`), an array of words to ignore.

func setWordFieldStringValue(String)

Sets the string that appears in the misspelled word field, using the string object `aString`.

func updateSpellingPanel(withMisspelledWord: String)

Causes the spell checker to update the Spelling panel’s misspelled-word field to reflect `word`.

func completions(forPartialWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Provides a list of complete words that the user might be trying to type based on a partial word in a given string.

func hasLearnedWord(String) -> Bool

Indicates whether the spell checker has learned a given word.

func unlearnWord(String)

Tells the spell checker to unlearn a given word.

func learnWord(String)

Adds the word to the spell checker dictionary.

func userQuotesArray(forLanguage: String) -> [String]

Returns the default values for quote replacement.

var userReplacementsDictionary: [String : String]

Returns the dictionary used when replacing words.

### Data Detector Interaction

func menu(for: NSTextCheckingResult, string: String, options: [NSSpellChecker.OptionKey : Any]?, atLocation: NSPoint, in: NSView) -> NSMenu?

Provides a menu containing contextual menu items suitable for certain kinds of detected results.

struct OptionKey

The constants are optional keys that can be used in the options dictionary parameter of the check(_:range:types:options:inSpellDocumentWithTag:orthography:wordCount:), requestChecking(of:range:types:options:inSpellDocumentWithTag:completionHandler:), and menu(for:string:options:atLocation:in:) methods.

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

enum CorrectionResponse

The correction response passed to therecord(_:toCorrection:forWord:language:inSpellDocumentWithTag:) method.

### Notifications

class let didChangeAutomaticSpellingCorrectionNotification: NSNotification.Name

This notification is posted when the spell checker did change text using automatic spell checking correction. The are posted to the application’s default notification center.

class let didChangeAutomaticTextReplacementNotification: NSNotification.Name

Posted when the spell checker changed text using automatic text replacement. This notification is posted to the app’s default notification center.

### Type Properties

class let didChangeAutomaticCapitalizationNotification: NSNotification.Name

class let didChangeAutomaticDashSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticPeriodSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticQuoteSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticTextCompletionNotification: NSNotification.Name

class var isAutomaticCapitalizationEnabled: Bool

class var isAutomaticDashSubstitutionEnabled: Bool

class var isAutomaticInlinePredictionEnabled: Bool

class var isAutomaticPeriodSubstitutionEnabled: Bool

class var isAutomaticQuoteSubstitutionEnabled: Bool

class var isAutomaticSpellingCorrectionEnabled: Bool

class var isAutomaticTextCompletionEnabled: Bool

class var isAutomaticTextReplacementEnabled: Bool

### Instance Methods

func deletesAutospaceBetweenString(String, andString: String, language: String?) -> Bool

func language(forWordRange: NSRange, in: String, orthography: NSOrthography?) -> String?

func preventsAutocorrection(before: String, language: String?) -> Bool

func requestCandidates(forSelectedRange: NSRange, in: String, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult]) -> Void)?) -> Int

func showInlinePrediction(forCandidates: [NSTextCheckingResult], client: any NSTextInputClient)

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

### Spell-checking

protocol NSChangeSpelling

A protocol that responder objects can implement to correct a misspelled word.

protocol NSIgnoreMisspelledWords

A protocol that enables the Ignore button in the Spelling panel to function properly.

