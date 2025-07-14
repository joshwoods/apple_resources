

- AppKit
- NSTextFinderClient
-  replaceCharacters(in:with:) 

Instance Method

# replaceCharacters(in:with:)

Replaces the text in the specified range with the new string.

macOS

``` source
optional func replaceCharacters(
    in range: NSRange,
    with string: String
)
```

## Parameters 

`range`  

The specified range of the text to replace.

`string`  

The replacement string.

## Discussion

See NSTextFinder for a complete description.

## See Also

### Replacing Text

func shouldReplaceCharacters(inRanges: [NSValue], with: [String]) -> Bool

Returns whether the specified strings should be replaced.

func didReplaceCharacters()

Specifies whether text characters were replaced.

