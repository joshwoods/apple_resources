

- Natural Language
- NLTokenizer
-  enumerateTokens(in:using:) 

Instance Method

# enumerateTokens(in:using:)

Enumerates over a given range of the string and calls the specified block for each token.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func enumerateTokens(
    in range: Range,
    using block: (Range, NLTokenizer.Attributes) -> Bool
)
```

## Parameters 

`range`  

The range of the string to tokenize.

`block`  

The closure to call after each token; return false if processing should stop.

## See Also

### Enumerating the tokens

func tokens(for: Range&lt;String.Index>) -> [Range&lt;String.Index>]

Tokenizes the string within the provided range.

func tokenRange(at: String.Index) -> Range&lt;String.Index>

Finds the range of the token at the given index.

func tokenRange(for: Range&lt;String.Index>) -> Range&lt;String.Index>

Finds the entire range of all tokens contained completely or partially within the specified range.

