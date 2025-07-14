

- Natural Language
- NLTagger
-  tokenRange(for:unit:) 

Instance Method

# tokenRange(for:unit:)

Finds the entire range of all tokens of the specified linguistic unit contained completely or partially within the specified range.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
func tokenRange(
    for range: Range,
    unit: NLTokenUnit
) -> Range
```

## Parameters 

`range`  

The range within the string to search for tokens.

`unit`  

The linguistic unit. For possible values, see NLTokenUnit.

## Return Value

The smallest possible range that contains all of the tokens of the specified linguistic unit within the range specified in `range`. This result includes a token’s entire range if any part of that token is included within `range`. If the length of `range` is 0, this return value is equivalent to tokenRangeAtIndex:unit:.

## See Also

### Determining the range of a unit token

func tokenRange(at: String.Index, unit: NLTokenUnit) -> Range&lt;String.Index>

Returns the range of the linguistic unit containing the specified character index.

enum NLTokenUnit

Constants representing linguistic units.

