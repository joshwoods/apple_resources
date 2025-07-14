

- AVFoundation
-  AVCaption 

Class

# AVCaption

An object that represents text to present over a time range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaption
```

## Overview

A caption contains a cue, which is a single sentence or paragraph of text for a time range in the video timeline. Within the active range, the caption may animate (for example, Karaoke lyrics) by rolling-up, changing visibility, or using other dynamic styling.

## Topics

### Creating a Caption

init(String, timeRange: CMTimeRange)

Creates a caption that contains text and a time range.

### Accessing Text and Timing

var text: String

The caption text.

var timeRange: CMTimeRange

The time range over which the system presents the caption.

### Accessing the Region

var region: AVCaptionRegion?

The region in which the caption exists.

### Accessing Font Styles

func fontStyle(at: String.Index) -> (AVCaption.FontStyle, Range&lt;String.Index>)

Returns the font style and range at the index position.

enum FontStyle

Font styles for caption text.

func fontWeight(at: String.Index) -> (AVCaption.FontWeight, Range&lt;String.Index>)

Returns the font weight and range at the index position.

enum FontWeight

Font weights for a caption.

func decoration(at: String.Index) -> (AVCaption.Decoration, Range&lt;String.Index>)

Returns the text decoration at the index position.

struct Decoration

Text decorations for caption text.

### Accessing Colors

func textColor(at: String.Index) -> (CGColor?, Range&lt;String.Index>)

Returns the text color at the index position.

func backgroundColor(at: String.Index) -> (CGColor?, Range&lt;String.Index>)

Returns the background color at the index position.

### Accessing Alignment

var textAlignment: AVCaption.TextAlignment

The alignment for the caption text.

enum TextAlignment

Text alignment options for a caption.

### Accessing Animation

var animation: AVCaption.Animation

The animation that the system applies to this caption.

enum Animation

Animation options for a caption.

### Accessing Advanced Typography

func ruby(at: String.Index) -> (AVCaption.Ruby?, Range&lt;String.Index>)

Returns the ruby text at the index position.

class Ruby

An object that presents ruby characters.

func textCombine(at: String.Index) -> (AVCaption.TextCombine, Range&lt;String.Index>)

Returns the text combine at the index position.

enum TextCombine

The caption’s supported rendering policy options.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableCaption

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

class AVMutableCaption

A mutable caption subclass that you use to create new captions.

