

- UIKit
- UIFontMetrics
-  init(forTextStyle:) 

Initializer

# init(forTextStyle:)

Creates a font metrics object for the specified text style.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(forTextStyle textStyle: UIFont.TextStyle)
```

## Parameters 

`textStyle`  

The text style that you want to apply to the font. For example, you might specify body for your app’s main content.

## Return Value

An initialized font metrics object.

## See Also

### Creating a Font Metrics Object

class var `default`: UIFontMetrics

The default font metrics object for content.

struct TextStyle

Constants that describe the preferred styles for fonts.

