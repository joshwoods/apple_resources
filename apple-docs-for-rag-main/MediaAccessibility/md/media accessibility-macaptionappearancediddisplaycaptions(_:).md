

- Media Accessibility
-  MACaptionAppearanceDidDisplayCaptions(\_:) 

Function

# MACaptionAppearanceDidDisplayCaptions(\_:)

Informs accessibility clients when captions display onscreen.

iOS 17.0+iPadOS 17.0+Mac Catalyst 13.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceDidDisplayCaptions(_ strings: CFArray)
```

## See Also

### General settings

let kMACaptionAppearanceSettingsChangedNotification: CFString

A notification that occurs when any user-defined caption settings change.

func MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferences for captioning sounds.

func MACaptionAppearanceGetDisplayType(MACaptionAppearanceDomain) -> MACaptionAppearanceDisplayType

Returns the preferred type of captions to display.

func MACaptionAppearanceSetDisplayType(MACaptionAppearanceDomain, MACaptionAppearanceDisplayType)

Sets the preference for the type of caption.

