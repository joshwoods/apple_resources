

- Bundle Resources
- Entitlements
-  com.apple.developer.networking.multicast 

Property List Key

# com.apple.developer.networking.multicast

A Boolean value that indicates whether an app can send or receive IP multicast traffic.

iOS 14.0+iPadOS 14.0+visionOS 1.0+

## Details 

Type  

boolean

## Discussion

Your app must have this entitlement to send or receive IP multicast or broadcast on iOS. It also allows your app to browse and advertise arbitrary Bonjour service types.

This entitlement requires permission from Apple before you can use it in your app. Request permission from the Multicast Networking Entitlement Request page.

## See Also

### Networking

Network Extensions Entitlement

The APIs an app can use to customize networking features.

**Key:** com.apple.developer.networking.networkextension

Personal VPN Entitlement

The API an app can use to create and control a custom system VPN configuration.

**Key:** com.apple.developer.networking.vpn.api

Associated Domains Entitlement

The associated domains for specific services, such as shared web credentials, universal links, and App Clips.

**Key:** com.apple.developer.associated-domains

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

