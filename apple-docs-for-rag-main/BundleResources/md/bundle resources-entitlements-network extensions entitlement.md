

- Bundle Resources
- Entitlements
-  Network Extensions Entitlement 

Property List Key

# Network Extensions Entitlement

The APIs an app can use to customize networking features.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 17.0+visionOS 1.0+

## Details 

Key  
com.apple.developer.networking.networkextension

Type  

array of strings

## Possible Values 

`dns-proxy`  

The APIs you use to proxy DNS queries.

`app-proxy-provider`  

The APIs you use to proxy TCP and UDP connections.

`content-filter-provider`  

The filter APIs you use to allow or deny network connections created by other apps on the system.

`packet-tunnel-provider`  

The APIs you use to tunnel IP packets to a remote network using any custom tunneling protocol.

`dns-proxy-systemextension`  

The APIs you use to proxy DNS queries, when signed with a Developer ID profile.

`app-proxy-provider-systemextension`  

The APIs you use to proxy TCP and UDP connections, when signed with a Developer ID profile.

`content-filter-provider-systemextension`  

The filter APIs you use to allow or deny network connections created by other apps on the system, when signed with a Developer ID profile.

`packet-tunnel-provider-systemextension`  

The APIs you use to tunnel IP packets to a remote network using any custom tunneling protocol, when signed with a Developer ID profile.

`dns-settings`  

The APIs you use to create and manage a system-wide DNS configuration.

`app-push-provider`  

The APIs you use for providing functionality similar to Apple Push Notification Service when access to the wider internet is unavailable.

`relay`  

The APIs you use to relay TCP and UDP connections, when signed with a Developer ID profile.

## Discussion

To add this entitlement to an App Store app, enable the Network Extensions capability in Xcode.

To add this entitlement to a macOS app distributed outside of the Mac App Store, perform the following steps:

1.  In the Certificates, Identifiers and Profiles section of the developer site, enable the Network Extension capability for your Developer ID–signed app. Generate a new provisioning profile and download it.

2.  On your Mac, drag the downloaded provisioning profile to Xcode to install it.

3.  In your Xcode project, enable manual signing and select the provisioning profile downloaded earlier and its associated certificate.

4.  Update the project’s `entitlements.plist` to include the `com.apple.developer.networking.networkextension` key and the values of the entitlement.

## See Also

### Networking

Personal VPN Entitlement

The API an app can use to create and control a custom system VPN configuration.

**Key:** com.apple.developer.networking.vpn.api

Associated Domains Entitlement

The associated domains for specific services, such as shared web credentials, universal links, and App Clips.

**Key:** com.apple.developer.associated-domains

com.apple.developer.networking.multicast

A Boolean value that indicates whether an app can send or receive IP multicast traffic.

com.apple.developer.associated-domains.applinks.read-write

A Boolean value that indicates whether the app can use universal links.

com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

5G Network Slicing App Category

The key that defines the app category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.appcategory

5G Network Slicing Traffic Category

The key that defines the traffic category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.trafficcategory

com.apple.developer.networking.vmnet

