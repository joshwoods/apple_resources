

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  textEffect 

Type Property

# textEffect

An attribute that applies a text effect to the text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let textEffect: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSString object. Use this attribute to specify a text effect, such as letterpressStyle. The default value of this property is `nil`, indicating no text effect.

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

static let textHighlightColorScheme: NSAttributedString.Key

The custom highlight color to apply to the text.

static let textHighlightStyle: NSAttributedString.Key

An attribute that adds a highlight color to the text to emphasize it.

static let textItemTag: NSAttributedString.Key

The name of a custom tag associated with a text item.

static let toolTip: NSAttributedString.Key

The tooltip text.

