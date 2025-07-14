

- Media Accessibility
-  MACaptionAppearanceCopySelectedLanguages(\_:) 

Function

# MACaptionAppearanceCopySelectedLanguages(\_:)

Returns the preferred caption languages.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopySelectedLanguages(_ domain: MACaptionAppearanceDomain) -> Unmanaged
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

## Return Value

An ordered array of preferred canonical language identifiers.

## Discussion

Languages added using the MACaptionAppearanceAddSelectedLanguage(_:_:) function are normalized. As a result, the contents of the returned array may have slightly different strings from those passed into MACaptionAppearanceAddSelectedLanguage(_:_:).

## See Also

### Language settings

func MACaptionAppearanceAddSelectedLanguage(MACaptionAppearanceDomain, CFString) -> Bool

Adds a preference for caption language to the stack of languages.

