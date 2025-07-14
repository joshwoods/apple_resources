

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  spellingState 

Type Property

# spellingState

The spelling state of the text.

macOS 10.0+

``` source
static let spellingState: NSAttributedString.Key
```

## Discussion

The value of this attribute is an integer. The default value of this key is 0, which indicates that there are no grammar or spelling errors. Specify a different value to indicate that a spelling or grammar error exists.

This key is available in macOS 10.2 and later, but its interpretation changed in OS X v10.5. Previously, any non-zero value caused the spelling indicator to be displayed. For macOS 10.5 and later, the (integer) value is treated as being composed of the spelling and grammar flags. See `NSSpellingStateAttributeName Flags` for possible values.

## See Also

### Getting text attribute keys

static let cursor: NSAttributedString.Key

The cursor object.

static let link: NSAttributedString.Key

The link for the text.

static let markedClauseSegment: NSAttributedString.Key

The index of the marked clause segment.

static let replacementIndex: NSAttributedString.Key

The replacement position associated with a format string specifier.

static let shadow: NSAttributedString.Key

The shadow of the text.

static let suggestionHighlight: NSAttributedString.Key

A highlight associated with a Spotlight suggestion.

static let textAlternatives: NSAttributedString.Key

The alternatives for the text.

static let textEffect: NSAttributedString.Key

An attribute that applies a text effect to the text.

static let textHighlightColorScheme: NSAttributedString.Key

The custom highlight color to apply to the text.

static let textHighlightStyle: NSAttributedString.Key

An attribute that adds a highlight color to the text to emphasize it.

static let textItemTag: NSAttributedString.Key

The name of a custom tag associated with a text item.

static let toolTip: NSAttributedString.Key

The tooltip text.

