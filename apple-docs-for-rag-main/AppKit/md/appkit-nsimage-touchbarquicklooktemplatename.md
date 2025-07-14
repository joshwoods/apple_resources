

- AppKit
- NSImage
-  touchBarQuickLookTemplateName 

Type Property

# touchBarQuickLookTemplateName

A template image for opening an item in Quick Look.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
class let touchBarQuickLookTemplateName: String
```

## Discussion

Touch Bar template images are exclusively for use in NSTouchBarItem objects and not in onscreen windows.

Use template images for your `NSTouchBarItem` images because, in the Touch Bar, template images respond automatically to system white-point changes.

## See Also

### Using template images

class let touchBarAddDetailTemplateName: String

A template image for showing additional detail for an item.

class let touchBarAddTemplateName: String

A template image for creating a new item.

class let touchBarAlarmTemplateName: String

A template image for setting or showing an alarm.

class let touchBarAudioInputMuteTemplateName: String

A template image for muting audio input or denoting that audio input is muted.

class let touchBarAudioInputTemplateName: String

A template image for denoting audio input.

class let touchBarAudioOutputMuteTemplateName: String

A template image for muting audio output or for denoting that audio output is muted.

class let touchBarAudioOutputVolumeHighTemplateName: String

A template image for setting the audio output volume to a high level, or for denoting that the audio is at the peak volume.

class let touchBarAudioOutputVolumeLowTemplateName: String

A template image for setting the audio output volume to a low level, or for denoting that it is set to a low level.

class let touchBarAudioOutputVolumeMediumTemplateName: String

A template image for setting the audio output volume to a medium level, or for denoting that it is set to a medium level.

class let touchBarAudioOutputVolumeOffTemplateName: String

A template image for setting the audio output volume to silent, or for denoting that it is set to silent.

class let touchBarBookmarksTemplateName: String

A template image for showing app-specific bookmarks.

class let touchBarColorPickerFillName: String

A template image for showing a color picker so the user can select a fill color.

class let touchBarColorPickerFontName: String

A template image for showing a color picker so the user can select a text color.

class let touchBarColorPickerStrokeName: String

A template image for showing a color picker so the user can select a stroke color.

class let touchBarCommunicationAudioTemplateName: String

A template image for initiating or denoting audio communication.

