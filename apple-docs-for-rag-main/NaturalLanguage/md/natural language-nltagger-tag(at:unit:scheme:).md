

- Natural Language
- NLTagger
-  tag(at:unit:scheme:) 

Instance Method

# tag(at:unit:scheme:)

Finds a tag for a given linguistic unit, for a single scheme, at the specified character position.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func tag(
    at index: String.Index,
    unit: NLTokenUnit,
    scheme: NLTagScheme
) -> (NLTag?, Range)
```

## Parameters 

`unit`  

The linguistic unit. See NLTokenUnit for possible values.

`scheme`  

The tag scheme. See NLTagScheme for possible values.

## Return Value

The tag for the requested tag scheme and linguistic unit, or `nil`. If a tag is returned, this function returns by reference the range of the token to `tokenRange`.

## See Also

### Getting linguistic tags

func tags(in: Range&lt;String.Index>, unit: NLTokenUnit, scheme: NLTagScheme, options: NLTagger.Options) -> [(NLTag?, Range&lt;String.Index>)]

Finds an array of linguistic tags and token ranges for a given string range and linguistic unit.

func tagHypotheses(at: String.Index, unit: NLTokenUnit, scheme: NLTagScheme, maximumCount: Int) -> ([String : Double], Range&lt;String.Index>)

Finds multiple possible tags for a given linguistic unit, for a single scheme, at the specified character position.

