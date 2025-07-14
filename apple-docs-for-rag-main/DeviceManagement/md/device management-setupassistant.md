

- Device Management
-  SetupAssistant 

Device Management Profile

# SetupAssistant

The payload you use to configure setup-assistant settings.

iOS 14.0+iPadOS 14.0+macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object SetupAssistant
```

## Properties

`SkipAccessibility`

`boolean`

Deprecated 

If `true`, the system skips the Accessibility pane.

Default: `false`

`SkipAppearance`

`boolean`

Deprecated 

If `true`, the system skips the Choose Your Look pane.

Default: `false`

`SkipCloudSetup`

`boolean`

Deprecated 

If `true`, the system skips the Apple ID setup pane.

Default: `false`

`SkipiCloudStorageSetup`

`boolean`

Deprecated 

If `true`, the system skips the iCloud Storage pane.

Default: `false`

`SkipPrivacySetup`

`boolean`

Deprecated 

If `true`, the system skips the Privacy consent pane.

Default: `false`

`SkipScreenTime`

`boolean`

Deprecated 

If `true`, the system skips the Screen Time pane.

Default: `false`

`SkipSiriSetup`

`boolean`

Deprecated 

If `true`, the system skips the Siri setup pane.

Default: `false`

`SkipSetupItems`

`[string]`

An array strings that describe the setup items to skip. SkipKeys provides a list of valid strings and their meanings. Available in iOS 14 and later.

`SkipTouchIDSetup`

`boolean`

Deprecated 

If `true`, the system skips the Touch ID setup pane.

Default: `false`

`SkipTrueTone`

`boolean`

Deprecated 

If `true`, the system skips the True Tone Display pane.

Default: `false`

`SkipUnlockWithWatch`

`boolean`

Deprecated 

If `true`, the system skips the Unlock With Apple Watch pane.

Default: `false`

`SkipWallpaper`

`boolean`

Deprecated 

Default: `false`

## Discussion

Specify `com.apple.SetupAssistant.managed` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS                   |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | iOS                     |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | \-                      |
| Allow Multiple Payloads    | \-                      |

### Profile Example

```

    PayloadContent

            SkipCloudSetup

            SkipSiriSetup

            SkipPrivacySetup

            SkipiCloudStorageSetup

            SkipTrueTone

            SkipAppearance

            SkipTouchIDSetup

            SkipScreenTime

            SkipAccessibility

            PayloadIdentifier
            com.example.mysetupassistantpayload
            PayloadType
            com.apple.SetupAssistant.managed
            PayloadUUID
            0dfccedc-e28f-4df5-bca7-a0807deab543
            PayloadVersion
            1

    PayloadDisplayName
    Setup Assistant
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4a66b685-604a-4558-92c7-ae3e082cf0ae
    PayloadVersion
    1

```

## See Also

### User Experience

object Accessibility

The payload you use to configure the accessibility features of the device.

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

object TimeMachine

The payload you use to configure Time Machine.

