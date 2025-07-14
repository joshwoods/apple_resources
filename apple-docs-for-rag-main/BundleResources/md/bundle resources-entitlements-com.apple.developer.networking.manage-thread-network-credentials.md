

- Bundle Resources
- Entitlements
-  com.apple.developer.networking.manage-thread-network-credentials 

Property List Key

# com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

iOS 15.0+iPadOS 15.0+visionOS 1.0+

## Details 

Type  

boolean

## Discussion

Use this entitlement while developing and testing your app. Update your Xcode project by opening the Capabilities library to add Managed Thread Network Credentials (development) to your app.

Once you’re ready to publish your app, request distribution permission for this entitlement from the ThreadNetwork Framework Entitlement Request page. If approved, go to the Developer Portal and enable the assigned Manage Thread Network Credentials entitlement that includes the new distribution access.

For implementation issues and questions about API and tools, please submit a support request.

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

com.apple.developer.networking.multicast

A Boolean value that indicates whether an app can send or receive IP multicast traffic.

com.apple.developer.associated-domains.applinks.read-write

A Boolean value that indicates whether the app can use universal links.

5G Network Slicing App Category

The key that defines the app category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.appcategory

5G Network Slicing Traffic Category

The key that defines the traffic category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.trafficcategory

com.apple.developer.networking.vmnet

