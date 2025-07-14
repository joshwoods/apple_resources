

- Device Management
-  Relay 

Device Management Profile

# Relay

The payload you use to configure relay settings.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object Relay
```

## Properties

`ExcludedDomains`

`[string]`

A list of domain strings to exclude from routing through the servers in `Relays`. Any connection that matches a domain in the list exactly or is a subdomain of the listed domain won’t use the relay server.

`MatchDomains`

`[string]`

A list of domain strings that the system uses to determine which connection to route through the servers in `Relays`.

Any connection that matches a domain in the list exactly or is a subdomain of the listed domain uses the relay servers, unless it matches a domain in `ExcludedDomains`.

If this list is empty, the system routes traffic to all domains to the relay servers, except those that match an excluded domain.

`Relays`

`[`Relay.Relay`]`

 (Required) 

An array of dictionaries that describe one or more relay servers that the system can chain together.

`RelayUUID`

`string`

A globally-unique identifier for this relay configuration. The system uses this UUID to route managed apps through the servers in `Relays`.

`Excluded FQDNs`

`[string]`

`MatchFQDNs`

`[string]`

## Topics

### Relay servers

object Relay.Relay

A dictionary that describes a relay server.

## See Also

### Networking

object Cellular

The payload you use to configure cellular settings.

object CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

object ContentCaching

The payload you use to configure the content-caching service.

object DNSSettings

The payload you use to configure encrypted DNS settings.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

