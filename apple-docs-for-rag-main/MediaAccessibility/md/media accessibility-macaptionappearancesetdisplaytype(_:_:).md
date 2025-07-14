

- Media Accessibility
-  MACaptionAppearanceSetDisplayType(\_:\_:) 

Function

# MACaptionAppearanceSetDisplayType(\_:\_:)

Sets the preference for the type of caption.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceSetDisplayType(
    _ domain: MACaptionAppearanceDomain,
    _ displayType: MACaptionAppearanceDisplayType
)
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

`displayType`  

A value representing options to use only forced captions, to allow system locale to override the language of the audio track, or to choose the best available captioning track from CC, SDH, or subtitles. See MACaptionAppearanceDisplayType.

## See Also

### General settings

let kMACaptionAppearanceSettingsChangedNotification: CFString

A notification that occurs when any user-defined caption settings change.

func MACaptionAppearanceDidDisplayCaptions(CFArray)

Informs accessibility clients when captions display onscreen.

func MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferences for captioning sounds.

func MACaptionAppearanceGetDisplayType(MACaptionAppearanceDomain) -> MACaptionAppearanceDisplayType

Returns the preferred type of captions to display.

