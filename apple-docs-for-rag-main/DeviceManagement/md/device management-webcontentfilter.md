

- Device Management
-  WebContentFilter 

Device Management Profile

# WebContentFilter

The payload you use to configure web content filters.

iOS 7.0+iPadOS 7.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object WebContentFilter
```

## Properties

`AllowListBookmarks`

`[`WebContentFilter.AllowListBookmarksItem`]`

An array of dictionaries that define the pages that the user can bookmark or visit. Use when `FilterType` is `BuiltIn`.

`AutoFilterEnabled`

`boolean`

If `true`, the system enables automatic filtering. Use when `FilterType` is `BuiltIn`.

Default: `false`

`ContentFilterUUID`

`string`

A globally unique identifier for this content filter configuration. The content filter processes network traffic for managed apps with the same `ContentFilterUUID` in their app attributes. Use when `FilterType` is `Plugin`.

`DenyListURLs`

`[string]`

An array of URLs that are inaccessible. Use when `FilterType` is `BuiltIn`.

`FilterBrowsers`

`boolean`

If `true`, the system enables filtering WebKit traffic. Use when `FilterType` is `Plugin`.

Note

At least one of `FilterBrowsers` or `FilterSockets` needs to be `true`.

Default: `false`

`FilterDataProviderBundleIdentifier`

`string`

The bundle identifier string of the filter data provider system extension. This string identifies the filter data provider when the filter starts running. Required if `FilterSockets` is `true`.

`FilterDataProviderDesignatedRequirement`

`string`

The designated requirement string that the system embeds in the code signature of the filter data provider system extension. This string identifies the filter data provider when the filter starts running. Required if `FilterSockets` is `true`.

`FilterGrade`

`string`

The system uses this value to derive the relative order of content filters. Filters with a grade of `firewall` see network traffic before filters with a grade of `inspector`. However, the system doesn’t define the order of filters within a grade.

Default: `firewall`

Possible Values: `firewall, inspector`

`FilterPackets`

`boolean`

If `true` and `FilterType` is `Plugin`, the system enables filtering network packets. Use when `FilterType` is `Plugin`.

Note

At least one of `FilterPackets` or `FilterSockets` needs to be `true`.

Default: `false`

`FilterPacketProviderBundleIdentifier`

`string`

The bundle identifier string of the filter packet provider system extension. This string identifies the filter packet provider when the filter starts running. Required if `FilterPackets` is `true`.

`FilterPacketProviderDesignatedRequirement`

`string`

The designated requirement string that the system embeds in the code signature of the filter packet provider system extension. This string identifies the filter packet provider when the filter starts running. Required if `FilterPackets` is `true`.

`FilterSockets`

`boolean`

If `true`, enables the filtering of socket traffic. Use when `FilterType` is `Plugin`.

Note

At least one of `FilterBrowsers` or `FilterSockets` needs to be `true`.

Default: `false`

`FilterType`

`string`

The type of filter, built-in or plug-in. In macOS, the system only supports the plug-in value.

Default: `BuiltIn`

Possible Values: `BuiltIn, Plugin`

`Organization`

`string`

The organization string to pass to the third-party plug-in. Use when `FilterType` is `Plugin`.

`Password`

`string`

The password for the service. Use when `FilterType` is `Plugin`.

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile that the system uses to authenticate the user. Use when `FilterType` is `Plugin`.

`PermittedURLs`

`[string]`

An array or URLs that are accessible whether or not the automatic filter allows access. Use when `FilterType` is `BuiltIn`. Requires that `AutoFilterEnabled` is `true`.

`PluginBundleID`

`string`

The bundle ID of the plug-in that provides filtering service. Required when `FilterType` is `Plugin`. Otherwise, it ignores this value. Consult your filtering solution vendor to determine what to specify for this value. Required when `FilterType` is `Plugin`.

`ServerAddress`

`string`

The server address, which may be the IP address, hostname, or URL. Use when `FilterType` is `Plugin`.

`UserDefinedName`

`string`

The display name for this filtering configuration. Required when `FilterType` is `Plugin`.

`UserName`

`string`

The user name for the service. Use when `FilterType` is `Plugin`.

`VendorConfig`

WebContentFilter.VendorConfig

The custom dictionary that the filtering service plug-in needs. Use when `FilterType` is `Plugin`.

`BlacklistedURLs`

`[string]`

Deprecated 

Use `DenyListURLs` instead.

`WhitelistedBookmarks`

`[`WebContentFilter.WhitelistedBookmarksItem`]`

Deprecated 

Use `AllowListBookmarks` instead.

`HideDenyListURLs`

`boolean`

Default: `false`

## Discussion

Specify `com.apple.webcontent-filter` as the payload type.

The system matches URLs using string-based matching. A URL matches an allow list, deny list, or permitted list pattern if the exact characters of the pattern appear as a substring of the URL requested in the web browser. For example, if the system doesn’t allow `test.com/a`, it blocks `test.com/a`, `test.com/apple`, and `test.com/a/b`.

The system matches list entries that terminate with a `/` character explicitly; if the system blocks or allows `test.com/a/`, it blocks or allows `test.com/a` and `test.com/a/b`.

Matching discards a `www` subdomain prefix if present, so if the system doesn’t allow `www.test.com`, it also blocks `m.test.com`.

All filtering options are active simultaneously. The system only permits URLs and sites that pass all rules.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, Shared iPad, macOS |
| User Channel               | \-                      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | iOS                     |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | \-                      |
| Allow Multiple Payloads    | \-                      |

### Profile Example

```

    PayloadContent

            AutoFilterEnabled

            DenylistURLs

                https://notallowedname.company.com

            FilterBrowsers

            FilterSockets

            FilterType
            BuiltIn
            PermittedURLs

                https://example.company.com

            PayloadIdentifier
            com.example.mywebcontentfilterpayload
            PayloadType
            com.apple.webcontent-filter
            PayloadUUID
            fb5d598f-0a96-4b77-9702-9edfc3417601
            PayloadVersion
            1

    PayloadDisplayName
    Web Content Filter
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b510e0c6-dc81-4b62-88d0-6a3ef82925e7
    PayloadVersion
    1

```

## Topics

### Objects

object WebContentFilter.AllowListBookmarksItem

The bookmark in the allow list of the web content filter.

object WebContentFilter.VendorConfig

A custom dictionary for the filtering service plug-in.

object WebContentFilter.WhitelistedBookmarksItem

The bookmark in the allow list of the web content filter.

## See Also

### Web

object WebClip

The profile you use to configure web clips on the device.

