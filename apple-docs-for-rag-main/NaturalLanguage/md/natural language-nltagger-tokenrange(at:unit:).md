

- Natural Language
- NLTagger
-  tokenRange(at:unit:) 

Instance Method

# tokenRange(at:unit:)

Returns the range of the linguistic unit containing the specified character index.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func tokenRange(
    at index: String.Index,
    unit: NLTokenUnit
) -> Range
```

## Parameters 

`unit`  

The linguistic unit. For possible values, see NLTokenUnit.

## Return Value

The range of the substring for the linguistic unit.

## See Also

### Determining the range of a unit token

func tokenRange(for: Range&lt;String.Index>, unit: NLTokenUnit) -> Range&lt;String.Index>

Finds the entire range of all tokens of the specified linguistic unit contained completely or partially within the specified range.

enum NLTokenUnit

Constants representing linguistic units.

