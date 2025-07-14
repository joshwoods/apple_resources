

- Natural Language
- NLTagger
-  tags(in:unit:scheme:options:) 

Instance Method

# tags(in:unit:scheme:options:)

Finds an array of linguistic tags and token ranges for a given string range and linguistic unit.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func tags(
    in range: Range,
    unit: NLTokenUnit,
    scheme: NLTagScheme,
    options: NLTagger.Options = []
) -> [(NLTag?, Range)]
```

## Parameters 

`range`  

The range from which to return tags.

`unit`  

The linguistic unit. See NLTokenUnit for possible values.

`scheme`  

The tag scheme. See NLTagScheme for possible values.

`options`  

The linguistic tagger options to use. See NLTagger.Options for possible values.

## Return Value

An array of the tags in the requested range.

## Discussion

When the returned array contains an entry that doesn’t have a corresponding tag scheme, that entry is an empty string (””).

## See Also

### Getting linguistic tags

func tag(at: String.Index, unit: NLTokenUnit, scheme: NLTagScheme) -> (NLTag?, Range&lt;String.Index>)

Finds a tag for a given linguistic unit, for a single scheme, at the specified character position.

func tagHypotheses(at: String.Index, unit: NLTokenUnit, scheme: NLTagScheme, maximumCount: Int) -> ([String : Double], Range&lt;String.Index>)

Finds multiple possible tags for a given linguistic unit, for a single scheme, at the specified character position.

