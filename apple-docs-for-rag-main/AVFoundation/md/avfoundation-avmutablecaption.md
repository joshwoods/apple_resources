

- AVFoundation
-  AVMutableCaption 

Class

# AVMutableCaption

A mutable caption subclass that you use to create new captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVMutableCaption
```

## Topics

### Configuring Text and Timing

var text: String

The caption text.

var timeRange: CMTimeRange

The time range over which the system presents the caption.

### Configuring the Region

var region: AVCaptionRegion

The region in which the caption exists.

### Configuring Font Styles

enum FontStyle

Font styles for caption text.

func setFontStyle(AVCaption.FontStyle, in: NSRange)

Sets the font style for a range of text.

func removeFontStyle(in: NSRange)

Removes a font style from a range of text.

enum FontWeight

Font weights for a caption.

func setFontWeight(AVCaption.FontWeight, in: NSRange)

Sets the font weight for a range of text.

func removeFontWeight(in: NSRange)

Removes a font weight from a range of text.

struct Decoration

Text decorations for caption text.

func setDecoration(AVCaption.Decoration, in: NSRange)

Sets a decoration for a range of text.

func removeDecoration(in: NSRange)

Removes a decoration from a range of text.

### Configuring Colors

func setTextColor(CGColor, in: NSRange)

Sets the text color for a range of text.

func removeTextColor(in: NSRange)

Removes the text color for a range of text.

func setBackgroundColor(CGColor, in: NSRange)

Sets the background color for a range of text.

func removeBackgroundColor(in: NSRange)

Removes a background color from a range of text.

### Configuring Alignment

var textAlignment: AVCaption.TextAlignment

The alignment of the caption text.

enum TextAlignment

Text alignment options for a caption.

### Configuring Animation

var animation: AVCaption.Animation

Animations to apply to the caption text.

enum Animation

Animation options for a caption.

### Configuring Advanced Typography

class Ruby

An object that presents ruby characters.

func setRuby(AVCaption.Ruby, in: NSRange)

Sets ruby text for a range.

func removeRuby(in: NSRange)

Removes ruby text from a range.

enum TextCombine

The caption’s supported rendering policy options.

func setTextCombine(AVCaption.TextCombine, in: NSRange)

Sets text combine for a range.

func removeTextCombine(in: NSRange)

Removes text combine from a range.

## Relationships

### Inherits From

- AVCaption

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Captions

class AVCaption

An object that represents text to present over a time range.

