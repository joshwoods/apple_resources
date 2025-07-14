

- AppKit
- NSSpellChecker
- NSSpellChecker.OptionKey
-  referenceDate 

Type Property

# referenceDate

An NSDate to be associated with the document, used as a referent for relative dates; if not specified, the current date will be used.

macOS 10.6+

``` source
static let referenceDate: NSSpellChecker.OptionKey
```

## See Also

### Spell Checker Options

static let documentAuthor: NSSpellChecker.OptionKey

An NSString containing the name of an author to be associated with the document

static let documentTitle: NSSpellChecker.OptionKey

An NSString containing the title to be associated with the document.

static let documentURL: NSSpellChecker.OptionKey

An NSURL to be associated with the document.

static let orthography: NSSpellChecker.OptionKey

An NSOrthography instance indicating an orthography to be used as a starting point for orthography checking, or as the orthography if orthography checking is not enabled.

static let quotes: NSSpellChecker.OptionKey

An NSArray containing four strings to be used with quote (opening double quote, closing double quote, opening single quote, and closing single quote in that order); if not specified, values will be taken from user’s preferences.

static let referenceTimeZone: NSSpellChecker.OptionKey

An NSTimeZone to be associated with the document, used as a reference for dates without time zones; if not specified, the current time zone will be used.

static let regularExpressions: NSSpellChecker.OptionKey

static let replacements: NSSpellChecker.OptionKey

An NSDictionary containing replacements to be used with NSTextCheckingTypeReplacement; if not specified, values will be taken from user’s preferences.

static let selectedRange: NSSpellChecker.OptionKey

