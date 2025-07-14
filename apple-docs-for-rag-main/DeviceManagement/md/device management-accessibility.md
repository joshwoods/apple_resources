

- Device Management
-  Accessibility 

Device Management Profile

# Accessibility

The payload you use to configure the accessibility features of the device.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object Accessibility
```

## Properties

`closeViewFarPoint`

`integer`

The minimum zoom level in the Zoom options.

`closeViewHotkeysEnabled`

`boolean`

If `true`, enables “Use keyboard shortcuts” in the Zoom options.

Default: `false`

`closeViewNearPoint`

`integer`

The maximum zoom level in the Zoom options.

`closeViewScrollWheelToggle`

`boolean`

If `true`, enables “Use scroll gesture” in the Zoom options.

Default: `false`

`closeViewShowPreview`

`boolean`

Deprecated 

If `true`, enables “Show preview rectangle” in the Zoom options. Only available in macOS 10.15 and earlier.

Default: `false`

`closeViewSmoothImages`

`boolean`

If `true`, enables “Smooth images” in the Zoom options.

Default: `false`

`contrast`

`number`

The contrast value in the Display options.

Minimum: `0`

Maximum: `1`

`flashScreen`

`boolean`

If `true`, enables “Flash the screen” in the Audio options.

Default: `false`

`grayscale`

`boolean`

Deprecated 

If `true`, enables “Use grayscale” in the Display options.

This option is deprecated in macOS 11.

Default: `false`

`mouseDriver`

`boolean`

If `true`, enables Mouse Keys in the Mouse & Trackpad options.

Default: `false`

`mouseDriverCursorSize`

`integer`

The size of the cursor.

`mouseDriverIgnoreTrackpad`

`boolean`

If `true`, ignores the built-in trackpad.

Default: `false`

`mouseDriverInitialDelay`

`integer`

The initial delay before moving the mouse with Mouse Keys.

`mouseDriverMaxSpeed`

`integer`

The maximum speed for the cursor when using Mouse Keys.

`slowKey`

`boolean`

If `true`, enables “Slow Keys” in the Keyboard options.

Default: `false`

`slowKeyBeepOn`

`boolean`

If `true`, enables “click key sounds” for Slow Keys.

Default: `false`

`slowKeyDelay`

`integer`

The acceptance delay, in milliseconds, for Slow Keys.

`stereoAsMono`

`boolean`

If `true`, plays stereo audio as mono.

Default: `false`

`stickyKey`

`boolean`

If `true`, enables Sticky Keys in the Keyboard options.

Default: `false`

`stickyKeyBeepOnModifier`

`boolean`

If `true`, enables the beep when a modifier key is set for Sticky Keys.

Default: `false`

`stickyKeyShowWindow`

`boolean`

If `true`, enables “Display pressed keys on screen” for Sticky Keys.

Default: `false`

`voiceOverOnOffKey`

`boolean`

If `true`, enables Voice Over.

Default: `false`

`whiteOnBlack`

`boolean`

If `true`, enables Invert Colors in Display Accommodations.

Default: `false`

## Discussion

Specify `com.apple.universalaccess` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            stickyKey

            PayloadIdentifier
            com.example.myaccessibilitypayload
            PayloadType
            com.apple.universalaccess
            PayloadUUID
            bff2939d-cb4c-4f6d-8521-e26bc7c03e96
            PayloadVersion
            1

    PayloadDisplayName
    Accessibility
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    e7b55cc7-0d94-4045-8868-dcc1b1c58159
    PayloadVersion
    1

```

## See Also

### User Experience

object Desktop

The payload you use to configure the desktop.

object Dock

The payload you use to configure the dock.

object Finder

The payload you use to configure Finder settings.

object HomeScreenLayout

The payload you use to configure the Home screen layout.

object ManagedMenuExtras

The payload you use to configure menu extras.

object Notifications

The payload you use to configure notifications.

object ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

object SetupAssistant

The payload you use to configure setup-assistant settings.

object TimeMachine

The payload you use to configure Time Machine.

