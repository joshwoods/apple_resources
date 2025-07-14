

- Core Text
-  CTLineCreateWithAttributedString(\_:) 

Function

# CTLineCreateWithAttributedString(\_:)

Creates a single immutable line object from an attributed string.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineCreateWithAttributedString(_ attrString: CFAttributedString) -> CTLine
```

## Parameters 

`attrString`  

The string that creates the line.

## Return Value

A reference to a CTLine object.

## Discussion

This function allows clients to create a line without creating a CTTypesetter object. The framework provides a typesetter for single-line typesetting under the hood. Simple elements that don’t require line breaks, such as text labels, can use this API.

## See Also

### Related Documentation

func CTTypesetterCreateWithAttributedString(CFAttributedString) -> CTTypesetter

Creates an immutable typesetter object using an attributed string.

func CTTypesetterCreateWithAttributedStringAndOptions(CFAttributedString, CFDictionary?) -> CTTypesetter?

Creates an immutable typesetter object using an attributed string and a dictionary of options.

func CTTypesetterCreateLine(CTTypesetter, CFRange) -> CTLine

Creates an immutable line from the typesetter.

### Creating Lines

func CTLineCreateTruncatedLine(CTLine, Double, CTLineTruncationType, CTLine?) -> CTLine?

Creates a truncated line from an existing line.

func CTLineCreateJustifiedLine(CTLine, CGFloat, Double) -> CTLine?

Creates a justified line from an existing line.

