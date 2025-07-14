

- AppKit
- NSTextFinderClient
-  shouldReplaceCharacters(inRanges:with:) 

Instance Method

# shouldReplaceCharacters(inRanges:with:)

Returns whether the specified strings should be replaced.

macOS

``` source
optional func shouldReplaceCharacters(
    inRanges ranges: [NSValue],
    with strings: [String]
) -> Bool
```

## Parameters 

`ranges`  

The ranges of the strings to replace.

`strings`  

The replacement strings.

## Return Value

Returns true if the replacement should occur; otherwise false.

## Discussion

See NSTextFinder for a complete description.

## See Also

### Replacing Text

func replaceCharacters(in: NSRange, with: String)

Replaces the text in the specified range with the new string.

func didReplaceCharacters()

Specifies whether text characters were replaced.

