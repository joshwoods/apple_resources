

- UIKit
- UIButton
- UIButton.Configuration
-  titleLineBreakMode 

Instance Property

# titleLineBreakMode

The line break mode the button uses to lay out the button’s title.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var titleLineBreakMode: NSLineBreakMode { get set }
```

## Discussion

Word and character wrapping modes enable multiline text, while other modes restrict the text to a single line.

The default value is NSLineBreakMode.byWordWrapping.

## See Also

### Configuring titles

var title: String?

The text of the title label the button displays.

var subtitle: String?

The text the subtitle label of the button displays.

var attributedTitle: AttributedString?

The text and style attributes for the button’s title label.

var attributedSubtitle: AttributedString?

The text and style attributes for the button’s subtitle label.

var titleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed title when the button state changes.

var subtitleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed subtitle when the button state changes.

struct UIConfigurationTextAttributesTransformer

Defines a text transformation that can affect the visual appearance of a string.

var titlePadding: CGFloat

The distance between the title and subtitle labels.

var titleAlignment: UIButton.Configuration.TitleAlignment

The text alignment the button uses to lay out the title and subtitle.

enum TitleAlignment

Specifies how to align a button’s title and subtitle.

var subtitleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s subtitle.

