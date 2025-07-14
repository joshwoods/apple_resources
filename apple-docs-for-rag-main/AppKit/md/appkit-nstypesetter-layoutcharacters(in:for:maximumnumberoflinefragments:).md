

- AppKit
- NSTypesetter
-  layoutCharacters(in:for:maximumNumberOfLineFragments:) 

Instance Method

# layoutCharacters(in:for:maximumNumberOfLineFragments:)

Lays out characters in the given character range for the specified layout manager.

macOS 10.5+

``` source
func layoutCharacters(
    in characterRange: NSRange,
    for layoutManager: NSLayoutManager,
    maximumNumberOfLineFragments maxNumLines: Int
) -> NSRange
```

## Parameters 

`characterRange`  

The range of the characters to lay out.

`layoutManager`  

The layout manager that does the drawing.

`maxNumLines`  

The maximum number of line fragments to lay out. Specify `NSUIntegerMax` for unlimited number of line fragments.

## Return Value

The method returns the actual character range that the receiving `NSTypesetter` processed.

## Discussion

The layout process can be interrupted when the number of line fragments exceeds `maxNumLines`.

