

- Media Accessibility
-  MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(\_:) 

Function

# MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(\_:)

Returns the preferences for captioning sounds.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(_ domain: MACaptionAppearanceDomain) -> Unmanaged
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

## Return Value

An array containing the preferred media characteristics for captioning of music, sounds, and dialog. See Captions.

## See Also

### General settings

let kMACaptionAppearanceSettingsChangedNotification: CFString

A notification that occurs when any user-defined caption settings change.

func MACaptionAppearanceDidDisplayCaptions(CFArray)

Informs accessibility clients when captions display onscreen.

func MACaptionAppearanceGetDisplayType(MACaptionAppearanceDomain) -> MACaptionAppearanceDisplayType

Returns the preferred type of captions to display.

func MACaptionAppearanceSetDisplayType(MACaptionAppearanceDomain, MACaptionAppearanceDisplayType)

Sets the preference for the type of caption.

