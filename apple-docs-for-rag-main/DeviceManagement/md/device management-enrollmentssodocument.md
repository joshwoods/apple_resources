

- Device Management
-  EnrollmentSSODocument 

Object

# EnrollmentSSODocument

Enrollment SSO streamlines the MDM enrollment process, reduces sign-ins, and improves security.

iOS 16.0+iPadOS 16.0+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object EnrollmentSSODocument
```

## Properties

`AppIDs`

`[string]`

An array of App IDs that specify apps that Enrollment SSO developer mode can use. In Enrollment SSO documents delivered through the developer endpoint, this key must be present and contain at least one value. In Enrollment SSO documents delivered by the standard Enrollment SSO endpoint, this key must not be present.

`AssociatedDomains`

`[string]`

An array of associated domains that the device uses with the Enrollment SSO extension.

`AssociatedDomainsEnableDirectDownloads`

`boolean`

If `true,` allows the domain to directly verify site association, instead of at Apple’s servers. Use this verification only with domains that are inaccessible on the public Internet.

Default: `false`

`ConfigurationProfile`

`data`

The profile containing an ExtensibleSingleSignOn payload that specifies the SSO extension in the downloaded app prior to enrollment. This profile may contain certificate payloads.

`Declarations`

`[data]`

`iTunesStoreID`

`integer`

The iTunes Store ID of the app to download prior to enrollment, to support Enrollment SSO during enrollment. Using developer mode ignores this key.

## See Also

### Essentials

Onboarding users with account sign-in

Examine new, user-initiated, identity-focused flows.

Discover Authentication Servers

Get a list of available authentication servers.

