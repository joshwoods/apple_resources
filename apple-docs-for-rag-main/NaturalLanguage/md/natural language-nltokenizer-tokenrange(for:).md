

- Natural Language
- NLTokenizer
-  tokenRange(for:) 

Instance Method

# tokenRange(for:)

Finds the entire range of all tokens contained completely or partially within the specified range.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
func tokenRange(for range: Range) -> Range
```

## Parameters 

`range`  

The range within the string to search for tokens.

## Return Value

The smallest possible range that contains all of the tokens within the range specified in `range`. This result includes a token’s entire range if any part of that token is included within `range`. If the length of `range` is 0, this return value is equivalent to tokenRange(at:).

## See Also

### Enumerating the tokens

func enumerateTokens(in: Range&lt;String.Index>, using: (Range&lt;String.Index>, NLTokenizer.Attributes) -> Bool)

Enumerates over a given range of the string and calls the specified block for each token.

func tokens(for: Range&lt;String.Index>) -> [Range&lt;String.Index>]

Tokenizes the string within the provided range.

func tokenRange(at: String.Index) -> Range&lt;String.Index>

Finds the range of the token at the given index.

