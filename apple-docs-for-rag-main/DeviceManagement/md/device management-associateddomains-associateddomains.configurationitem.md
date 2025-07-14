

- Device Management
- AssociatedDomains
-  AssociatedDomains.ConfigurationItem 

Device Management Profile

# AssociatedDomains.ConfigurationItem

A dictionary that maps apps to their associated domains.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object AssociatedDomains.ConfigurationItem
```

## Properties

`ApplicationIdentifier`

`string`

 (Required) 

The app identifier to associate the domains with.

`AssociatedDomains`

`[string]`

 (Required) 

The domains to associate with the app. Each string is in the form of “`service:domain`”. Use fully qualified hostnames, such as `www.example.com`. See Supporting associated domains for more information.

`EnableDirectDownloads`

`boolean`

If `true`, the system enables direct download of data for this domain instead of through a CDN. Set the entitlement value for this domain to `service:domain?mode=managed`; otherwise, the system ignores this value. Available in macOS 11 and later.

Default: `false`

