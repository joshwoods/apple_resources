

- Device Management
-  WebClip 

Device Management Profile

# WebClip

The profile you use to configure web clips on the device.

iOS 4.0+iPadOS 4.0+macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object WebClip
```

## Properties

`FullScreen`

`boolean`

If `true`, the system launches the web clip as a full-screen web app.

Default: `false`

`Icon`

`data`

The PNG icon to show on the Home screen. If not set, the system displays a white square. For best results, provide a square image that’s no larger than 400 x 400 pixels and less than 1 MB when uncompressed. The graphics file is automatically scaled and cropped to fit, if necessary, and converted to PNG format. Web clip icons are 144 x 144 pixels for iPad devices with a Retina display, and 114 x 114 pixels for iPhone devices. To prevent the device from adding a shine to the image, set `Precomposed` to `true`.

`IgnoreManifestScope`

`boolean`

If `true`, a full screen web clip can navigate to an external web site without showing Safari UI. Otherwise, Safari UI appears when navigating away from the web clip’s URL. This key has no effect when `FullScreen` is `false`. Available in iOS 14 and later.

Default: `false`

`IsRemovable`

`boolean`

If `true`, the system enables removing the web clip.

Default: `true`

`Label`

`string`

 (Required) 

The name of the web clip that the system displays on the Home screen.

`Precomposed`

`boolean`

If `true`, the system prevents SpringBoard from adding shine to the icon.

Default: `false`

`TargetApplicationBundleIdentifier`

`string`

The application bundle identifier of the application that opens the URL. To use this property, install the profile through MDM. Available in iOS 14 and later.

`URL`

`string`

 (Required) 

The URL of the web clip.

## Discussion

Specify `com.apple.webClip.managed` as the payload type.

Use this payload to add web clips to the Home screen of the user’s iOS device or to the Dock on a Mac. Web clips provide fast access to favorite webpages.

For iOS devices, if you prevent the user from removing the web clip, the only way to remove it is to remove the configuration profile that installed it. Also, for iOS devices it must have a display name and an icon URL for the payload to be valid.

A full-screen web clip on iOS devices opens the URL as a web app without a browser; there’s no URL, search bar, or bookmarks.

For Shared iPad devices, the system supports this payload on the user channel only.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS                     |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS, macOS, Shared iPad |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad |

### Profile Example

```

    PayloadContent

            FullScreen

            IgnoreManifestScope

            IsRemovable

            Label
            Example
            Precomposed

            URL
            example.com
            PayloadIdentifier
            com.example.mywebclippayload
            PayloadType
            com.apple.webClip.managed
            PayloadUUID
            1d6d6912-708e-441a-9272-526ef05bbe3c
            PayloadVersion
            1

    PayloadDisplayName
    Web Clip
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    289fc7fc-2870-479d-b30f-8d0592b7ef04
    PayloadVersion
    1

```

## See Also

### Web

object WebContentFilter

The payload you use to configure web content filters.

