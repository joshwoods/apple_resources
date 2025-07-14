

- Device Management
-  Dock 

Device Management Profile

# Dock

The payload you use to configure the dock.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Dock
```

## Properties

`AllowDockFixupOverride`

`boolean`

If `true`, use the file in `/Library/Preferences/com.apple.dockfixup.plist` when a new user or migrated user logs in. This option has no effect for existing users. Available in macOS 10.12 and later. Only available on the device channel.

Default: `false`

`autohide`

`boolean`

If `true`, enables “Automatically hide and show the dock.”

Default: `false`

`autohide-immutable`

`boolean`

If `true`, locks “Automatically hide.”

Default: `false`

`contents-immutable`

`boolean`

If `true`, disables changes to the dock.

Default: `false`

`dblclickbehavior`

`string`

The behavior when the window’s title bar is double-clicked.

Possible Values: `minimize, maximize, none`

`dblclickbehavior-immutable`

`boolean`

If `true`, locks “Double-click a window’s title bar.”

Default: `false`

`largesize`

`integer`

The size of the largest magnification.

Minimum: `16`

Maximum: `128`

`launchanim`

`boolean`

If `true`, enables “Animate opening applications.”

Default: `false`

`launchanim-immutable`

`boolean`

If `true`, locks “Animate opening applications.”

Default: `false`

`magnification`

`boolean`

If `true`, enables magnification.

Default: `false`

`magnify-immutable`

`boolean`

If `true`, locks magnification.

Default: `false`

`magsize-immutable`

`boolean`

If `true`, locks the magnification slider.

Default: `false`

`MCXDockSpecialFolders`

`[string]`

One or more special folders that may be created at user login time and placed in the dock.

The “My Applications” item is only used for Simple Finder environments. The “Original Network Home” item is only used for mobile account users.

Possible Values: `AddDockMCXMyApplicationsFolder, AddDockMCXDocumentsFolder, AddDockMCXSharedFolder, AddDockMCXOriginalNetworkHomeFolder`

`mineffect`

`string`

The minimize effect.

Possible Values: `genie, scale`

`mineffect-immutable`

`boolean`

If `true`, locks “Minimize windows using.”

Default: `false`

`minimize-to-application`

`boolean`

If `true`, enables “Minimize windows into application icon.”

Default: `false`

`minintoapp-immutable`

`boolean`

If `true`, disables the “Minimize windows into application icon” checkbox.

Default: `false`

`orientation`

`string`

The orientation of the dock.

Possible Values: `bottom, left, right`

`persistent-apps`

`[`Dock.StaticItem`]`

An array of items located on the Applications side of the Dock that can be removed from the dock.

`persistent-others`

`[`Dock.StaticItem`]`

An array of items located on the Documents side of the Dock that can be removed from the dock.

`position-immutable`

`boolean`

If `true`, locks the position.

Default: `false`

`show-process-indicators`

`boolean`

If true, shows the process indicator.

Default: `false`

`showindicators-immutable`

`boolean`

If `true`, locks “Show indicators.”

Default: `false`

`show-recents`

`boolean`

If `true`, enables “Show recent items.”

Default: `false`

`showrecents-immutable`

`boolean`

If `true`, disables “Show recent applications” checkbox.

Default: `false`

`size-immutable`

`boolean`

If `true`, locks the size slider.

Default: `false`

`static-apps`

`[`Dock.StaticItem`]`

An array of items located on the Applications side of the Dock and cannot be removed from that location.

`static-only`

`boolean`

If `true`, uses the `static-apps` and `static-others` dictionaries for the dock and ignores any items in the `persistent-apps` and `persistent-others` dictionaries. If `false`, the contents are merged with the static items listed first.

Default: `false`

`static-others`

`[`Dock.StaticItem`]`

An array of items located on the Documents side of the Dock and cannot be removed from that location.

`tilesize`

`integer`

The tile size. Values must be in the range from 16 to 128.

Minimum: `16`

Maximum: `128`

`windowtabbing`

`string`

Set the “Prefer tabs when opening documents” to the provided value.

Possible Values: `manual, always, fullscreen`

`windowtabbing-immutable`

`boolean`

If `true`, disables “Prefer tabs when opening documents” checkbox.

Default: `false`

## Discussion

Specify `com.apple.dock` as the payload type.

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

            tilesize
            40
            size-immutable

            magnification

            magnify-immutable

            largesize
            100
            magsize-immutable

            orientation
            left
            position-immutable

            mineffect
            genie
            mineffect-immutable

            windowtabbing
            manual
            windowtabbing-immutable

            dblclickbehavior
            maximize
            dblclickbehavior-immutable

            minimize-to-application

            minintoapp-immutable

            launchanim

            launchanim-immutable

            autohide

            autohide-immutable

            show-process-indicators

            showindicators-immutable

            show-recents

            showrecents-immutable

            PayloadIdentifier
            com.example.mydockpayload
            PayloadType
            com.apple.dock
            PayloadUUID
            8d443602-52f2-48ff-aaa9-35b16c7c54c9
            PayloadVersion
            1

    PayloadDisplayName
    Dock
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    c139d3e0-5468-43b0-90bf-5e05b2e8cd6f
    PayloadVersion
    1

```

## Topics

### Objects

object Dock.StaticItem

Items that are located on the Documents side of the Dock and cannot be removed from that location.

object Dock.StaticItem.Tile-data

The dictionary that contains details about a dock item.

object Dock.StaticItem.Tile-data.File-data

For Apple use only.

## See Also

### User Experience

object Accessibility

The payload you use to configure the accessibility features of the device.

object Desktop

The payload you use to configure the desktop.

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

