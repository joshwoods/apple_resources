

- Network Extension
- NETunnelProviderManager
-  appRules 

Instance Property

# appRules

The rules for specific apps in a per-app VPN.

macOS 10.15.4+

``` source
var appRules: [NEAppRule] { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

For per-app VPNs only, the system routes network traffic originating from an app that matches one of these rules through the VPN.

## See Also

### Configuring a per-app VPN

class func forPerAppVPN() -> Self

Returns a tunnel provider manager for managing a per-app VPN configuration.

var excludedDomains: [String]

The domains that the system excludes from a per-app VPN.

var associatedDomains: [String]

The domains that the system routes network traffic through for a per-app VPN.

var calendarDomains: [String]

The calendar servers that the system routes connections from the Calendar app through for a per-app VPN.

var contactsDomains: [String]

The contacts servers that the system routes connections from the Contacts app through for a per-app VPN.

var mailDomains: [String]

The mail servers that the system routes connections from the Mail app through for a per-app VPN.

var safariDomains: [String]

The website domains that the system routes connections from the Safari app through a per-app VPN.

