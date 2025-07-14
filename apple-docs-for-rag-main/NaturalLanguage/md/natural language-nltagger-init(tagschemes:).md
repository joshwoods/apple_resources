

- Natural Language
- NLTagger
-  init(tagSchemes:) 

Initializer

# init(tagSchemes:)

Creates a linguistic tagger instance using the specified tag schemes and options.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(tagSchemes: [NLTagScheme])
```

## Parameters 

`tagSchemes`  

An array of tag schemes to be used. See NLTagScheme for the possible values.

## Discussion

Pass any tag schemes to tagSchemes that you intend to use with the methods described in Enumerating linguistic tags and Getting linguistic tags in NLTagger.

Tip

Avoid specifying tag schemes that you won’t use to ensure optimal performance.

## See Also

### Creating a tagger

var string: String?

The string being analyzed by the linguistic tagger.

