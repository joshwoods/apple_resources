

- Media Accessibility
-  MACaptionAppearanceAddSelectedLanguage(\_:\_:) 

Function

# MACaptionAppearanceAddSelectedLanguage(\_:\_:)

Adds a preference for caption language to the stack of languages.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceAddSelectedLanguage(
    _ domain: MACaptionAppearanceDomain,
    _ language: CFString
) -> Bool
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

`language`  

A canonical language identifier (see doc://com.apple.documentation/documentation/corefoundation/cflocale-rsj) of the preferred caption language.

## Return Value

Returns `true` if addition was successful; `false` if an error occurred. Errors are most likely the result of invalid language codes.

## Discussion

The added language will appear in the array returned by MACaptionAppearanceCopySelectedLanguages(_:). Call the `MACaptionAppearanceAddSelectedLanguage` function anytime a user selects a specific captioning language from a pop-up menu or other UI affordance. For example, an AVFoundation client may execute the following code:

```
```

## See Also

### Language settings

func MACaptionAppearanceCopySelectedLanguages(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferred caption languages.

