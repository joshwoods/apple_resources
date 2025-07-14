

- Media Accessibility
-  kMACaptionAppearanceSettingsChangedNotification 

Global Variable

# kMACaptionAppearanceSettingsChangedNotification

A notification that occurs when any user-defined caption settings change.

iOS 17.0+iPadOS 17.0+Mac Catalyst 13.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
let kMACaptionAppearanceSettingsChangedNotification: CFString
```

## See Also

### General settings

func MACaptionAppearanceDidDisplayCaptions(CFArray)

Informs accessibility clients when captions display onscreen.

func MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferences for captioning sounds.

func MACaptionAppearanceGetDisplayType(MACaptionAppearanceDomain) -> MACaptionAppearanceDisplayType

Returns the preferred type of captions to display.

func MACaptionAppearanceSetDisplayType(MACaptionAppearanceDomain, MACaptionAppearanceDisplayType)

Sets the preference for the type of caption.

