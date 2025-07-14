

- UIKit
- UIContentUnavailableConfiguration
-  UIContentUnavailableConfiguration.TextProperties 

Structure

# UIContentUnavailableConfiguration.TextProperties

Properties to configure text for a content-unavailable view.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
struct TextProperties
```

## Topics

### Instance Properties

var adjustsFontSizeToFitWidth: Bool

A Boolean value indicating whether the view modifies the font size of the text to fit the available width.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that determines whether the view tightens text before truncating.

var color: UIColor

The color of the text.

var font: UIFont

The font of the text.

var lineBreakMode: NSLineBreakMode

The technique for wrapping and truncating the text.

var minimumScaleFactor: CGFloat

The minimum scale factor for the text.

var numberOfLines: Int

The maximum number of lines for the text.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable

