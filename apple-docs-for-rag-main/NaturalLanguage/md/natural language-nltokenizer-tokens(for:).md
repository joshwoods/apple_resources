

- Natural Language
- NLTokenizer
-  tokens(for:) 

Instance Method

# tokens(for:)

Tokenizes the string within the provided range.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func tokens(for range: Range) -> [Range]
```

## Parameters 

`range`  

The range within the string that should be tokenzied.

## Return Value

Returns the ranges corresponding to the tokens for the tokenizer’s unit that intersect the given range.

## See Also

### Enumerating the tokens

func enumerateTokens(in: Range&lt;String.Index>, using: (Range&lt;String.Index>, NLTokenizer.Attributes) -> Bool)

Enumerates over a given range of the string and calls the specified block for each token.

func tokenRange(at: String.Index) -> Range&lt;String.Index>

Finds the range of the token at the given index.

func tokenRange(for: Range&lt;String.Index>) -> Range&lt;String.Index>

Finds the entire range of all tokens contained completely or partially within the specified range.

