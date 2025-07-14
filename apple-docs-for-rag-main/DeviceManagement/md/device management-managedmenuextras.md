

- Device Management
-  ManagedMenuExtras 

Device Management Profile

# ManagedMenuExtras

The payload you use to configure menu extras.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ManagedMenuExtras
```

## Properties

`AirPort.menu`

`boolean`

If `true`, enables the AirPort menu extra.

`Battery.menu`

`boolean`

If `true`, enables the Battery menu extra.

`Bluetooth.menu`

`boolean`

If `true`, enables the Bluetooth menu extra.

`Clock.menu`

`boolean`

If `true`, enables the Clock menu extra.

`CPU.menu`

`boolean`

If `true`, enables the CPU menu extra.

`delaySeconds`

`number`

The number of seconds to delay after login before adding or removing menu extras. If the delay is too short, the menu extras don’t appear, or disappear from the menu bar.

Default: `2.5`

`Displays.menu`

`boolean`

If `true`, enables the Displays menu extra.

`Eject.menu`

`boolean`

If `true`, enables the Eject menu extra.

`Fax.menu`

`boolean`

If `true`, enables the Fax menu extra.

`HomeSync.menu`

`boolean`

If `true`, enables the HomeSync menu extra.

`iChat.menu`

`boolean`

If `true`, enables the iChat menu extra.

`Ink.menu`

`boolean`

If `true`, enables the Ink menu extra.

`IrDA.menu`

`boolean`

If `true`, enables the IrDA menu extra.

`maxWaitSeconds`

`number`

The maximum wait, in seconds, for all menu extras to be added or removed.

Default: `20`

`PCCard.menu`

`boolean`

If `true`, enables the PCCard menu extra.

`PPP.menu`

`boolean`

If `true`, enables the PPP menu extra.

`PPPoE.menu`

`boolean`

If `true`, enables the PPPoE menu extra.

`RemoteDesktop.menu`

`boolean`

If `true`, enables the Remote Desktop menu extra.

`Script Menu.menu`

`boolean`

If `true`, enables the Script menu extra.

`Spaces.menu`

`boolean`

If `true`, enables the Spaces menu extra.

`Sync.menu`

`boolean`

If `true`, enables the Sync menu extra.

`TextInput.menu`

`boolean`

If `true`, enables the Text Input menu extra.

`TimeMachine.menu`

`boolean`

If `true`, enables the TimeMachine menu extra.

`UniversalAccess.menu`

`boolean`

If `true`, enables the Universal Access menu extra.

`User.menu`

`boolean`

If `true`, enables the User menu extra.

`Volume.menu`

`boolean`

If `true`, enables the Volume menu extra.

`VPN.menu`

`boolean`

If `true`, enables the VPN menu extra.

`WWAN.menu`

`boolean`

If `true`, enables the WWAN menu extra.

## Discussion

Specify `com.apple.mcxMenuExtras` as the payload type.

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

            Battery.menu

            delaySeconds
            30
            maxWaitSeconds
            60
            PayloadIdentifier
            com.example.mymanagedmenuextraspayload
            PayloadType
            com.apple.mcxMenuExtras
            PayloadUUID
            93bd5b68-0141-4055-aaaf-a6cebc1cfeeb
            PayloadVersion
            1

    PayloadDisplayName
    Menu Extras
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    dc2618ce-736c-4af7-b652-f9cdf3eb9ce4
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

object Notifications

The payload you use to configure notifications.

object ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

object SetupAssistant

The payload you use to configure setup-assistant settings.

object TimeMachine

The payload you use to configure Time Machine.

