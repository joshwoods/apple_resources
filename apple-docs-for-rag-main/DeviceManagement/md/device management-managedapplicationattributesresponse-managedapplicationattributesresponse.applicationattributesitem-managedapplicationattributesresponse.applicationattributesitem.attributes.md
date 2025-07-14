

- Device Management
- ManagedApplicationAttributesResponse
- ManagedApplicationAttributesResponse.ApplicationAttributesItem
-  ManagedApplicationAttributesResponse.ApplicationAttributesItem.Attributes 

Device Management Command

# ManagedApplicationAttributesResponse.ApplicationAttributesItem.Attributes

A dictionary that contains a managed app’s attributes.

iOS 7.0+iPadOS 7.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationAttributesResponse.ApplicationAttributesItem.Attributes
```

## Properties

`AssociatedDomains`

`[string]`

This app’s associated domains. This value is available in iOS 13 and later.

`AssociatedDomainsEnableDirectDownloads`

`boolean`

If `true`, perform claimed site association verification directly at the domain instead of on Apple’s servers. Only set this to `true` for domains that can’t access the internet. This value is available in iOS 14 and later.

Default: `false`

`CellularSliceUUID`

`string`

`ContentFilterUUID`

`string`

The content Filter UUID assigned to this app.

Available in iOS 16 and later.

`DNSProxyUUID`

`string`

The DNS Proxy UUID assigned to this app.

Available in iOS 16 and later.

`Hideable`

`boolean`

Default: `true`

`Lockable`

`boolean`

Default: `true`

`RelayUUID`

`string`

The relay UUID for this app.

`Removable`

`boolean`

If `false`, this app isn’t removable while it’s a managed app. This value is available in iOS 14 and later.

Default: `true`

`TapToPayScreenLock`

`boolean`

Default: `false`

`VPNUUID`

`string`

A per-app VPN unique identifier for this app.

