

- Natural Language
- NLTokenizer
-  tokenRange(at:) 

Instance Method

# tokenRange(at:)

Finds the range of the token at the given index.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func tokenRange(at index: String.Index) -> Range
```

## Parameters 

`index`  

The location in the string that is of interest.

## Return Value

The range of the token at the given location.

## See Also

### Enumerating the tokens

func enumerateTokens(in: Range&lt;String.Index>, using: (Range&lt;String.Index>, NLTokenizer.Attributes) -> Bool)

Enumerates over a given range of the string and calls the specified block for each token.

func tokens(for: Range&lt;String.Index>) -> [Range&lt;String.Index>]

Tokenizes the string within the provided range.

func tokenRange(for: Range&lt;String.Index>) -> Range&lt;String.Index>

Finds the entire range of all tokens contained completely or partially within the specified range.

