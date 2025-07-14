

- UIKit
- NSTextContentStorageDelegate
-  textContentStorage(\_:textParagraphWith:) 

Instance Method

# textContentStorage(\_:textParagraphWith:)

Returns a custom paragraph for a range that you provide from the object’s attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func textContentStorage(
    _ textContentStorage: NSTextContentStorage,
    textParagraphWith range: NSRange
) -> NSTextParagraph?
```

## Parameters 

`textContentStorage`  

The object’s content manager.

`range`  

The NSRange that describes the extent of the string.

## Return Value

A new NSTextParagraph, or `nil`.

## Discussion

When non-`nil`, `textContentStorage` uses the text paragraph instead of creating the standard NSTextParagraph with the attributed substring in `range`. The attributed string for a custom text paragraph must have a length of `range.length`.

