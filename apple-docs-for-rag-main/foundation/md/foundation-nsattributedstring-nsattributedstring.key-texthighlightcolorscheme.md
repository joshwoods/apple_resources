

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  textHighlightColorScheme 

Type Property

# textHighlightColorScheme

The custom highlight color to apply to the text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static let textHighlightColorScheme: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSAttributedString.TextHighlightColorScheme structure. The default value of this attribute is `nil`, which applies the default system highlight color to the text when the textHighlightStyle attribute is present.

A highlight adds a background color behind the text, and applies a contrasting foreground color to the text itself. Set the value of this attribute to default, or don’t specify the attribute at all, to apply a highlight with the default system color. Specify a different value for this attribute to apply that highlight color instead.

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

static let spellingState: NSAttributedString.Key

The spelling state of the text.

static let suggestionHighlight: NSAttributedString.Key

A highlight associated with a Spotlight suggestion.

static let textAlternatives: NSAttributedString.Key

The alternatives for the text.

static let textEffect: NSAttributedString.Key

An attribute that applies a text effect to the text.

static let textHighlightStyle: NSAttributedString.Key

An attribute that adds a highlight color to the text to emphasize it.

static let textItemTag: NSAttributedString.Key

The name of a custom tag associated with a text item.

static let toolTip: NSAttributedString.Key

The tooltip text.

