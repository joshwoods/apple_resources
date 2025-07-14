

- Natural Language
- NLTagger
-  tagHypotheses(at:unit:scheme:maximumCount:) 

Instance Method

# tagHypotheses(at:unit:scheme:maximumCount:)

Finds multiple possible tags for a given linguistic unit, for a single scheme, at the specified character position.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
func tagHypotheses(
    at index: String.Index,
    unit: NLTokenUnit,
    scheme: NLTagScheme,
    maximumCount: Int
) -> ([String : Double], Range)
```

## Parameters 

`index`  

The position of the initial character.

`unit`  

The linguistic unit. See NLTokenUnit for possible values.

`scheme`  

The tag scheme. See NLTagScheme for possible values. Not all tag schemes produce more than one prediction.

`maximumCount`  

The maximum number of tag predictions to return.

## Return Value

A tuple containing a dictionary and a range.

## Discussion

Each dictionary entry is a predicted tag with its associated probability score. These tags are the top candidates proposed as possible tags for the token. The dictionary contains up to `maximumCount` entries.

The range contains the range of the individual token for which these tags were produced.

## See Also

### Getting linguistic tags

func tags(in: Range&lt;String.Index>, unit: NLTokenUnit, scheme: NLTagScheme, options: NLTagger.Options) -> [(NLTag?, Range&lt;String.Index>)]

Finds an array of linguistic tags and token ranges for a given string range and linguistic unit.

func tag(at: String.Index, unit: NLTokenUnit, scheme: NLTagScheme) -> (NLTag?, Range&lt;String.Index>)

Finds a tag for a given linguistic unit, for a single scheme, at the specified character position.

