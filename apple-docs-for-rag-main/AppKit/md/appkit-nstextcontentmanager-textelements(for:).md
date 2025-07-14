

- AppKit
- NSTextContentManager
-  textElements(for:) 

Instance Method

# textElements(for:)

Returns an array of text elements that intersect with the range you specify.

macOS 12.0+

``` source
func textElements(for range: NSTextRange) -> [NSTextElement]
```

## Parameters 

`range`  

An NSTextRange that describes the range of text to process.

## Return Value

An array of NSTextElement.

## Discussion

This method can return a set of elements that don’t fill the entire range if the entire range isn’t synchronously available. Uses enumerateTextElements(from:options:using:) to fill the array.

