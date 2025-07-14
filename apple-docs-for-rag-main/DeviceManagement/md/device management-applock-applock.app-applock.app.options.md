

- Device Management
- AppLock
- AppLock.App
-  AppLock.App.Options 

Device Management Profile

# AppLock.App.Options

The dictionary of options to set for the app.

iOS 6.0+iPadOS 6.0+tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object AppLock.App.Options
```

## Properties

`DisableAutoLock`

`boolean`

If `true`, the device doesn’t automatically go to sleep after an idle period.

Default: `false`

`DisableDeviceRotation`

`boolean`

If `true`, the system disables device rotation sensing.

Default: `false`

`DisableRingerSwitch`

`boolean`

If `true`, the system disables the ringer switch. When disabled, the ringer behavior depends on what position the switch was in when it was first disabled.

Default: `false`

`DisableSleepWakeButton`

`boolean`

If `true`, the system disables the sleep/wake button.

Default: `false`

`DisableTouch`

`boolean`

If `true`, the system disables the touch screen. In tvOS, it disables the touch surface on the Apple TV Remote.

Default: `false`

`DisableVolumeButtons`

`boolean`

If `true`, the system disables the volume buttons.

Default: `false`

`EnableAssistiveTouch`

`boolean`

If `true`, the system enables AssistiveTouch.

Default: `false`

`EnableInvertColors`

`boolean`

If `true`, the system enables Invert Colors.

Default: `false`

`EnableMonoAudio`

`boolean`

If `true`, the system enables Mono Audio.

Default: `false`

`EnableSpeakSelection`

`boolean`

If `true`, the system enables Speak Selection.

Default: `false`

`EnableVoiceOver`

`boolean`

If `true`, the system enables VoiceOver.

Default: `false`

`EnableZoom`

`boolean`

If `true`, the system enables Zoom.

Default: `false`

`EnableVoiceControl`

`boolean`

If `true`, the system enables Voice Control.

Default: `false`

## See Also

### Profiles

object AppLock.App.UserEnabledOptions

The dictionary of user-editable options to set for the app.

