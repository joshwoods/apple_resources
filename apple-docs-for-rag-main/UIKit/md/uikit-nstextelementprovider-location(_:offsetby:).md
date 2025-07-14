

- UIKit
- NSTextElementProvider
-  location(\_:offsetBy:) 

Instance Method

# location(\_:offsetBy:)

Returns a new location from location with offset you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func location(
    _ location: any NSTextLocation,
    offsetBy offset: Int
) -> (any NSTextLocation)?
```

## Parameters 

`location`  

An NSTextLocation in the text element.

`offset`  

An offset of the number of characters to or from `location`.

## Return Value

An new `NSTextLocation`, or `nil` of the offset exceeds the bounds of the text.

## See Also

### Accessing and updating the text

func enumerateTextElements(from: (any NSTextLocation)?, options: NSTextContentManager.EnumerationOptions, using: (NSTextElement) -> Bool) -> (any NSTextLocation)?

Enumerates text elements starting at the text location you provide.

**Required**

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func replaceContents(in: NSTextRange, with: [NSTextElement]?)

Replaces the characters specified by range with the text elements you provide.

**Required**

