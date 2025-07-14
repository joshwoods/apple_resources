

- Natural Language
- NLTagger
-  availableTagSchemes(for:language:) 

Type Method

# availableTagSchemes(for:language:)

Retrieves the tag schemes available for a particular unit (like word or sentence) and language on the current device.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class func availableTagSchemes(
    for unit: NLTokenUnit,
    language: NLLanguage
) -> [NLTagScheme]
```

## Parameters 

`unit`  

The linguistic unit. For possible values, see NLTokenUnit.

`language`  

The NLLanguage identifying the language.

## Return Value

The supported tag schemes. For possible values, see NLTagScheme.

## See Also

### Getting the tag schemes

class func requestAssets(for: NLLanguage, tagScheme: NLTagScheme, completionHandler: (NLTagger.AssetsResult, (any Error)?) -> Void)

Asks the Natural Language framework to load any missing assets for a tag scheme onto the device for the given language.

enum AssetsResult

The response to an asset request.

var tagSchemes: [NLTagScheme]

The tag schemes configured for this linguistic tagger.

struct NLTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

