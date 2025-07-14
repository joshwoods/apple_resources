

- AVFoundation
-  AVTextStyleRule 

Class

# AVTextStyleRule

An object that represents the text styling rules to apply to a media item’s textual content.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVTextStyleRule
```

## Overview

You use text style objects to format subtitles, closed captions, and other text-related content of the item. The system applies these rules to all or part of the text of the media item.

## Topics

### Creating and Initializing Style Rules

class func textStyleRules(fromPropertyList: Any) -> [AVTextStyleRule]?

Creates an array of text style rule objects from the specified property-list object.

convenience init?(textMarkupAttributes: [String : Any])

Creates a text style rule object with the specified style attributes.

init?(textMarkupAttributes: [String : Any], textSelector: String?)

Creates a text style rule object with the specified style attributes and text range information.

### Accessing the Style Attributes

var textMarkupAttributes: [String : Any]

A dictionary of text style attributes to apply to the text.

var textSelector: String?

A string that identifies the text to which the attributes should apply.

### Exporting the Style Rules

class func propertyList(for: [AVTextStyleRule]) -> Any

Converts one or more text style rules into a serializable property list object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Accessing Text Style Rules

var textStyleRules: [AVTextStyleRule]?

An array of text style rules that specify the formatting and presentation of Web Video Text Tracks (WebVTT) subtitles.

