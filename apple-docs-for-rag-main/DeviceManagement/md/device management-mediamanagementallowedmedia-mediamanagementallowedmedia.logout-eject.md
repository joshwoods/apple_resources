

- Device Management
- MediaManagementAllowedMedia
-  MediaManagementAllowedMedia.Logout-eject 

Device Management Profile

# MediaManagementAllowedMedia.Logout-eject

A dictionary of volumes to eject when the user logs out.

macOS 10.7–11.0DeprecatedDevice Assignment ServicesVPP License Management

``` source
object MediaManagementAllowedMedia.Logout-eject
```

## Properties

`all-media`

`string`

Deprecated 

Unused; set to an empty string.

`bd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`blankbd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`blankcd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`blankdvd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`cd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`disk-image`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`dvd`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`dvdram`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`harddisk-external`

`[string]`

Deprecated 

A string or an array of media action strings. Internally installed SD cards and USB flash drives are included in the hard disk-external category.

This key is the default for media types that don’t fall into other categories.

Possible Values: `authenticate, read-only, deny, eject`

`harddisk-internal`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

`networkdisk`

`[string]`

Deprecated 

A media action string or an array of media action strings.

Possible Values: `authenticate, read-only, deny, eject`

## Discussion

These are the valid media action strings:

`authenticate`: The user is authenticated before the media is mounted.

`read-only`: The media is mounted as read-only; this action cannot be combined with unmount controls.

`deny`: The media isn’t mounted.

`eject`: The media isn’t mounted and is ejected, if possible. Note that some volumes aren’t defined as ejectable, so using the deny key may be the best solution. This action cannot be combined with unmount controls.

## See Also

### Objects

object MediaManagementAllowedMedia.Mount-controls

A dictionary of volumes to control volume mounting.

object MediaManagementAllowedMedia.Unmount-controls

A dictionary to control volume unmounting.

