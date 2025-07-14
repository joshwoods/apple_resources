

- AppKit
- NSTextFinderClient
-  didReplaceCharacters() 

Instance Method

# didReplaceCharacters()

Specifies whether text characters were replaced.

macOS

``` source
optional func didReplaceCharacters()
```

## Discussion

See NSTextFinder for a complete description.

## See Also

### Replacing Text

func shouldReplaceCharacters(inRanges: [NSValue], with: [String]) -> Bool

Returns whether the specified strings should be replaced.

func replaceCharacters(in: NSRange, with: String)

Replaces the text in the specified range with the new string.

