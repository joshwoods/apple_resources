

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  replacementIndex 

Type Property

# replacementIndex

The replacement position associated with a format string specifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let replacementIndex: NSAttributedString.Key
```

## Discussion

When creating an attributed string from a format string and one or more replacement values, this attribute indicates the ordinal index of each replacement. You must specify the NSAttributedStringFormattingApplyReplacementIndexAttribute option at creation time to add this attribute to the substituted text. The value of this key is an `NSNumber` with the replacement position of the substitute text.

## See Also

### Getting text attribute keys

static let cursor: NSAttributedString.Key

The cursor object.

static let link: NSAttributedString.Key

The link for the text.

static let markedClauseSegment: NSAttributedString.Key

The index of the marked clause segment.

static let shadow: NSAttributedString.Key

The shadow of the text.

static let spellingState: NSAttributedString.Key

The spelling state of the text.

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

