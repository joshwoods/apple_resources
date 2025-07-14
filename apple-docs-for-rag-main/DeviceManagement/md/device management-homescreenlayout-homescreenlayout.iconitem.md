

- Device Management
- HomeScreenLayout
-  HomeScreenLayout.IconItem 

Device Management Profile

# HomeScreenLayout.IconItem

An array of dictionaries that conform to the icon dictionary format.

iOS 9.3+iPadOS 9.3+tvOS 11.0+Device Assignment ServicesVPP License Management

``` source
object HomeScreenLayout.IconItem
```

## Properties

`BundleID`

`string`

The bundle identifier of the app. This setting is required if the type is `Application`.

`DisplayName`

`string`

The human-readable string shown to the user. This setting is valid only if the type is `Folder`.

`Pages`

`[[`HomeScreenLayout.IconItem`]]`

An array of arrays of dictionaries, each conforming to the icon dictionary format. This setting is valid only if the type is `Folder`.

`Type`

`string`

 (Required) 

The type of the dock item.

Possible Values: `App, Folder, WebClip`

`URL`

`string`

The URL of the existing web clip for this item. This setting is required if `type` is `WebClip`. If more than one web clip exists with the same URL, the behavior is undefined.

Specifying a web clip in this payload doesn’t create the web clip. Use the WebClip payload to create a web clip.

## Discussion

This setting is ignored on tvOS.

