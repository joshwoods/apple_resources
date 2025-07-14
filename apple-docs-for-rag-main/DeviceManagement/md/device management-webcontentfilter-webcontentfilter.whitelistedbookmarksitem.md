

- Device Management
- WebContentFilter
-  WebContentFilter.WhitelistedBookmarksItem 

Device Management Profile

# WebContentFilter.WhitelistedBookmarksItem

The bookmark in the allow list of the web content filter.

iOS 7.0+iPadOS 7.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object WebContentFilter.WhitelistedBookmarksItem
```

## Properties

`Title`

`string`

Deprecated   (Required) 

The title of the bookmark.

`URL`

`string`

Deprecated   (Required) 

The URL of the bookmark in the allow list.

## Discussion

This device management profile adds any URLs in the allow list to the browser’s bookmarks. The browser prevents the user from visiting any sites not bookmarked. The number of bookmarks on the allow list should be limited to about 500.

## See Also

### Objects

object WebContentFilter.AllowListBookmarksItem

The bookmark in the allow list of the web content filter.

object WebContentFilter.VendorConfig

A custom dictionary for the filtering service plug-in.

