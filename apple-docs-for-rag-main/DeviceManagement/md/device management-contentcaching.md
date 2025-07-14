

- Device Management
-  ContentCaching 

Device Management Profile

# ContentCaching

The payload you use to configure the content-caching service.

macOS 10.13.4+Device Assignment ServicesVPP License Management

``` source
object ContentCaching
```

## Properties

`AllowCacheDelete`

`boolean`

If true, the system purges content from the cache automatically when it needs disk space for other apps when free disk space runs low on the computer. Set to `false` to maximize effectiveness of Content Caching. Available in macOS 10.15 and later.

Default: `true`

`AllowPersonalCaching`

`boolean`

If `true`, the system caches the user’s iCloud data. Changes to this value don’t have an immediate effect. Clients may take some time, such as hours or days, to react to changes.

Note

At least one of the `AllowPersonalCaching` or `AllowSharedCaching` keys need to be `true`.

Default: `true`

`AllowSharedCaching`

`boolean`

If `true`, the system caches non-iCloud content, such as apps and software updates. Changes to this value don’t have an immediate effect. Clients may take some time, such as hours or days, to react to changes.

Note

At least one of the `AllowPersonalCaching` or `AllowSharedCaching` keys need to be `true`.

Default: `true`

`AutoActivation`

`boolean`

If `true`, the system automatically activates the content cache when possible and prevents disabling it. If `allowContentCaching` is `false`, `AutoActivation` is also `false`.

Removing a profile that set `AutoActivation` to `true` doesn’t deactivate the Content Cache.

Default: `false`

`AutoEnableTetheredCaching`

`boolean`

If `true`, the system automatically enables Internet connection sharing when possible and prevent disabling Internet connection sharing. `DenyTetheredCaching` overrides `AutoEnableTetheredCaching`. Tethered caching requires Content Caching.

Available in macOS 10.15.4 and later.

Default: `false`

`CacheLimit`

`integer`

The maximum number of bytes of disk space to use for the content cache. Set to `0` for unlimited disk space.

Default: `0`

`DataPath`

`string`

The path to the directory used to store cached content. Changing this setting manually doesn’t automatically move cached content from the old location to the new one. To move content automatically, use the Sharing preference’s Content Caching pane. The value must be (or end with) `/Library/Application Support/Apple/AssetCache/Data`.

The system creates a directory and its intermediates for the given data path if it doesn’t already exist. The directory is owned by `_assetcache:_assetcache` and has mode 0750. Its immediate parent directory (`.../Library/Application Support/Apple/AssetCache`) is owned by `_assetcache:_assetcache` and has mode `0755`.

Default: `/Library/Application Support/Apple/AssetCache/Data`

`DenyTetheredCaching`

`boolean`

If `true`, the system disables tethered caching.

Default: `false`

`DisplayAlerts`

`boolean`

If `true`, Content Caching displays exceptional conditions (alerts) as system notifications in the upper corner of the screen. Alerts were automatically displayed starting in macOS 10.13. In macOS 10.15 the alerts are off by default, but still available through this setting. Available in macOS 10.15 and later.

Default: `false`

`KeepAwake`

`boolean`

If `true`, the system fprevents the computer from sleeping as long as Content Caching is on (System Preferences \> Sharing \> Content Caching is on). Customers who want Content Caching to be as available as musch as possible should turn this setting on. Available in macOS 10.15 and later.

Default: `false`

`ListenRanges`

`[`ContentCaching.Ranges`]`

An array of dictionaries that describe a range of client IP addresses to serve.

`ListenRangesOnly`

`boolean`

If `true`, the content cache provides content to the clients in the `ListenRanges`.

Default: `false`

`ListenWithPeersAndParents`

`boolean`

If `true`, the content cache provides content to the clients in the union of the `ListenRanges`, `PeerListenRanges` and `Parents`.

Default: `true`

`LocalSubnetsOnly`

`boolean`

If `true`, the content cache offers content to clients only on the same immediate local network only. No content is offered to clients on other networks reachable by the content cache. If `LocalSubnetsOnly` is `true`, the system ignores `ListenRanges`.

Default: `true`

`LogClientIdentity`

`boolean`

If `true`, the Content Cache logs the IP address and port number of the clients that request content.

Default: `false`

`ParentSelectionPolicy`

`string`

The policy to implement when choosing among more than one configured parent content cache. With every policy, the system skips parent caches that are temporarily unavailable. Allowed values:

`first-available`  
Always use the first available parent in the Parents list. Use this policy to designate permanent primary, secondary, and subsequent parents.

`url-path-hash`  
Hash the path part of the requested URL so that the same parent is always used for the same URL. This is useful for maximizing the size of the combined caches of the parents.

`random`  
Choose a parent at random. Use this policy for load balancing.

`round-robin`  
Rotate through the parents in order. Use this policy for load balancing.

`sticky-available`  
Use the first available parent in the Parents list until it becomes unavailable, then advance to the next one. Use this policy for designating floating primary, secondary, and subsequent parents.

Default: `round-robin`

Possible Values: `first-available, url-path-hash, random, round-robin, sticky-available`

`Parents`

`[string]`

An array of the local IP addresses of other content caches that this cache should download from or upload to, instead of downloading from or uploading to Apple directly. The system ignores invalid addresses and addresses of computers that aren’t content caches. The system skips Parent caches that become unavailable. If all parent content caches become unavailable, the content cache downloads from or uploads to Apple directly, until a parent content cache becomes available again.

`PeerFilterRanges`

`[`ContentCaching.Ranges`]`

An array of dictionaries describing a range of peer IP addresses that the content cache uses to filter its list of peers to query for content. The content cache only queries peers in `PeerFilterRanges`. When `PeerFilterRanges` is an empty array, the content cache doesn’t query any peers.

`PeerListenRanges`

`[`ContentCaching.Ranges`]`

An array of dictionaries describing a range of peer IP addresses the content cache responds to. When `PeerListenRanges` is an empty array, the content cache responds with an error to all cache queries.

`PeerLocalSubnetsOnly`

`boolean`

If `true`, the content cache only peers with other content caches on the same immediate local network, rather than with content caches that use the same public IP address as the device. When `PeerLocalSubnetsOnly` is `true`, it overrides the configuration of `PeerFilterRanges` and `PeerListenRanges`. If the network changes, the local network peering restrictions update appropriately. If `false`, the content cache defers to `PeerFilterRanges` and `PeerListenRanges` for configuring the peering restrictions.

Default: `true`

`Port`

`integer`

The TCP port number on which the content cache accepts requests for uploads or downloads. Set to `0` to pick a random, available port.

Default: `0`

`PublicRanges`

`[`ContentCaching.Ranges`]`

An array of dictionaries describing a range of public IP addresses that the cloud servers should use for matching clients to content caches.

## Discussion

Specify `com.apple.AssetCache.managed` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            AllowPersonalCaching

            AllowSharedCaching

            AutoActivation

            CacheLimit
            180000000000
            DenyTetheredCaching

            ListenRangesOnly

            LocalSubnetsOnly

            LogClientIdentity

            ParentSelectionPolicy
            round-robin
            PeerLocalSubnetsOnly

            Port
            0
            PayloadIdentifier
            com.example.mycontentcachingpayload
            PayloadType
            com.apple.AssetCache.managed
            PayloadUUID
            c7d8c850-e4ef-0135-0bd6-0c4de9ce4c04
            PayloadVersion
            1

    PayloadDisplayName
    Content Caching
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    a430c370-b5d5-4e5b-b46b-137931e8b230
    PayloadVersion
    1

```

## Topics

### Objects

object ContentCaching.Ranges

A range of IP addresses to cache.

## See Also

### Networking

object Cellular

The payload you use to configure cellular settings.

object CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

object DNSSettings

The payload you use to configure encrypted DNS settings.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

