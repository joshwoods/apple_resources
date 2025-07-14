

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  textHighlightStyle 

Type Property

# textHighlightStyle

An attribute that adds a highlight color to the text to emphasize it.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static let textHighlightStyle: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSAttributedString.TextHighlightStyle structure. The default value of this attribute is `nil`, which does not add a highlight to the text.

A highlight adds a background color behind the text, and adjusts the color of the text itself to contrast appropriately. The default highlight style applies the system highlight color to your text. To apply a different color, add the textHighlightColorScheme attribute to your text in addition to this one. Use the textHighlightColorScheme key to specify which highlight color you want.

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

static let textHighlightColorScheme: NSAttributedString.Key

The custom highlight color to apply to the text.

static let textItemTag: NSAttributedString.Key

The name of a custom tag associated with a text item.

static let toolTip: NSAttributedString.Key

The tooltip text.

