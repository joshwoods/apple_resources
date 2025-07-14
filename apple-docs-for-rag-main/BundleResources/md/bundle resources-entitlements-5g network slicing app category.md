

- Bundle Resources
- Entitlements
-  5G Network Slicing App Category 

Property List Key

# 5G Network Slicing App Category

The key that defines the app category entitlement to enable Cellular Network Slicing.

iOS 17.0+iPadOS 17.0+

## Details 

Key  
com.apple.developer.networking.slicing.appcategory

Type  

array of strings

## Possible Values 

`gaming-6014`  

Sets the application category for gaming apps.

`communication-9000`  

Sets the application category for communication apps.

`streaming-9001`  

Sets the application category for streaming apps.

## Discussion

To enable Cellular Network Slicing, also set the 5G Network Slicing Traffic Category entitlement.

Note

Cellular Network Slicing is only available on supported carriers. Check with individual carriers for availability.

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

com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

5G Network Slicing Traffic Category

The key that defines the traffic category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.trafficcategory

com.apple.developer.networking.vmnet

