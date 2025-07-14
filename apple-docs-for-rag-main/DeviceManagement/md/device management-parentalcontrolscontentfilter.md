

- Device Management
-  ParentalControlsContentFilter 

Device Management Profile

# ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsContentFilter
```

## Properties

`restrictWeb`

`boolean`

 (Required) 

If `true`, enables web content filters.

`useContentFilter`

`boolean`

If `true`, filters content automatically.

Default: `false`

`filterBlacklist`

`[string]`

The array of URLs that defines a deny list. When `restrictWeb` and `useContentFilter` are enabled, no URLs in the deny list are available to the user.

`filterWhitelist`

`[string]`

The array of URLs that defines an allow list. When `restrictWeb` and `useContentFilter` are enabled, only URLs in the allow list are available to the user.

`siteWhitelist`

`[`ParentalControlsContentFilter.SiteWhitelistItem`]`

An array of sites that defines an allow list. If specified, this defines additional allowed sites besides those in the automated allow list and deny list, including disallowed adult sites.

This key is required if `whiteListEnabled` is `true`.

`whitelistEnabled`

`boolean`

If `true`, enables web content filters.

Default: `false`

## Discussion

Specify `com.apple.familycontrols.contentfilter` as the payload type.

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

            filterWhitelist

                http://www.example.com

            filterBlacklist

                http://www.example2.com

            siteWhitelist

                    address
                    http://www.example3.com
                    bookmarkPath
                    /
                    pageTitle
                    example3

            restrictWeb

            useContentFilter

            whitelistEnabled

            PayloadIdentifier
            com.example.mycontentfilterpayload
            PayloadType
            com.apple.familycontrols.contentfilter
            PayloadUUID
            342c6863-6e3c-4e00-893e-f76757ae41c7
            PayloadVersion
            1

    PayloadDisplayName
    Parental Controls Content Filter
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    764e94bc-ab75-456f-ac47-3a1062e70ffb
    PayloadVersion
    1

```

## Topics

### Objects

object ParentalControlsContentFilter.SiteWhitelistItem

A dictionary defining a site for the allow list.

## See Also

### Parental Controls

object ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

object ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

object ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

object ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

