

- Device Management
-  HomeScreenLayout 

Device Management Profile

# HomeScreenLayout

The payload you use to configure the Home screen layout.

iOS 9.3+iPadOS 9.3+tvOS 11.0+Device Assignment ServicesVPP License Management

``` source
object HomeScreenLayout
```

## Properties

`Dock`

`[`HomeScreenLayout.IconItem`]`

An array of dictionaries, each of which must conform to the icon dictionary format. If this key isn’t present, the user’s dock is empty.

`Pages`

`[[`HomeScreenLayout.IconItem`]]`

 (Required) 

An array of arrays of dictionaries, each of which must conform to the icon dictionary format.

## Discussion

Specify `com.apple.homescreenlayout` as the payload type.

This payload defines a layout of apps, folders, and web clips for the Home screen. On iOS, this layout is locked and can’t be modified by the user.

If a home screen layout puts more than four items in the iPhone or iPod touch dock the location of the fifth and succeeding items may be undefined but they will not be omitted.

To disable deletion of apps, set `allowAppRemoval` to `false` with Restrictions.

### Profile Availability

|                            |                        |
|----------------------------|------------------------|
| Device Channel             | iOS, Shared iPad, tvOS |
| User Channel               | Shared iPad            |
| Allow Manual Install       | iOS, tvOS              |
| Requires Supervision       | iOS, tvOS              |
| Requires User Approved MDM | \-                     |
| Allowed in User Enrollment | \-                     |
| Allow Multiple Payloads    | \-                     |

### Profile Example

```

    PayloadContent

            Dock

                    Type
                    Application
                    BundleID
                    com.apple.mobilesafari

                    Type
                    Application
                    BundleID
                    com.apple.Preferences

                    Type
                    Folder
                    DisplayName
                    Example
                    Pages

                                Type
                                WebClip
                                DisplayName
                                Example
                                URL
                                companyname.com

                                Type
                                Application
                                BundleID
                                com.apple.News

            Pages

                        Type
                        Application
                        BundleID
                        com.apple.MobileSMS

                        Type
                        Application
                        BundleID
                        com.apple.camera

                        Type
                        Folder
                        DisplayName
                        Display Name exampler
                        Pages

                                    Type
                                    Application
                                    BundleID
                                    com.apple.podcasts

                        Type
                        WebClip
                        URL
                        https://www.apple.com
                        DisplayName
                        Custom Home Screen Layout

                        Type
                        Application
                        BundleID
                        com.apple.AppStore

                        Type
                        Folder
                        DisplayName
                        Important Folder

                        Type
                        Application
                        BundleID
                        com.apple.Bridge

            PayloadIdentifier
            com.example.myhomescreenlayoutpayload
            PayloadType
            com.apple.homescreenlayout
            PayloadUUID
            f0b2d13e-a985-4264-9901-707feabddfcd
            PayloadVersion
            1

    PayloadDisplayName
    Home Screen Layout
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    24c41ae0-f8a9-4d9f-a007-d67b0dc15af4
    PayloadVersion
    1

```

## Topics

### Objects

object HomeScreenLayout.IconItem

An array of dictionaries that conform to the icon dictionary format.

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

