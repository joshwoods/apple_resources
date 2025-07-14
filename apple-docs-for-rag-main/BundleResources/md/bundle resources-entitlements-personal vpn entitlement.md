

- Bundle Resources
- Entitlements
-  Personal VPN Entitlement 

Property List Key

# Personal VPN Entitlement

The API an app can use to create and control a custom system VPN configuration.

iOS 8.0+iPadOS 8.0+macOS 10.10+visionOS 1.0+

## Details 

Key  
com.apple.developer.networking.vpn.api

Type  

array of strings

## Possible Values 

`allow-vpn`  

## Discussion

With the Personal VPN Entitlement enabled, your app can use the NEVPNManager class to manage a Personal VPN configuration.

To add this entitlement to your app, enable the Personal VPN capability in Xcode. When the entitlement is enabled, Xcode sets the value to `allow-vpn`.

## See Also

### Networking

Network Extensions Entitlement

The APIs an app can use to customize networking features.

**Key:** com.apple.developer.networking.networkextension

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

