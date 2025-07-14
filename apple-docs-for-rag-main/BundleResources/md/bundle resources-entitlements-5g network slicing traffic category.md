

- Bundle Resources
- Entitlements
-  5G Network Slicing Traffic Category 

Property List Key

# 5G Network Slicing Traffic Category

The key that defines the traffic category entitlement to enable Cellular Network Slicing.

iOS 17.0+iPadOS 17.0+

## Details 

Key  
com.apple.developer.networking.slicing.trafficcategory

Type  

array of strings

## Possible Values 

`defaultslice-1`  

A service type for Cellular Network Slicing when not setting the other service types.

`video-2`  

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

`background-3`  

A service type for high-delay tolerant, high-loss tolerant, elastic flow, and variable size connections.

`voice-4`  

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

`callsignaling-5`  

A service for low-loss tolerant, inelastic-flow, jitter tolerant, bursty but short rate, and variable size connections.

`responsivedata-6`  

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

`avstreaming-7`  

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, variable rate, and size connections.

`responsiveav-8`  

A service type for low-delay tolerant, low-to-medium-loss tolerant, elastic flow, variable packet interval, rate, and size responsive (time-sensitive) connections.

## Discussion

To enable Cellular Network Slicing, you need to set the appropriate entitlements and properties.

Set this entitlement and the 5G Network Slicing App Category entitlement in your property list. If you don’t entitle your app by specifying both these entitlements, your apps network connections won’t use Cellular Network Slicing, even if supported by the carrier.

Use this array to define the different slice types your app’s entitled to. For example, if your app opens network connections using the network service types video, voice, and call signaling, the entitlement property must include `video-2`, `voice-4,` and `callsignaling-5` values for this entitlement key.

Also set one of the following properties, depending on your app’s networking implementation:

- Set serviceClass when using the Networking framework.

- Set networkServiceType when using URLSessionConfiguration.

- Set networkServiceType when using URLRequest.

If your app uses sockets, set this entitlement to `defaultslice-1`. With sockets, all your app traffic uses a slice defined by the carrier to accept all traffic categories. You should still set the 5G Network Slicing App Category entitlement.

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

5G Network Slicing App Category

The key that defines the app category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.appcategory

com.apple.developer.networking.vmnet

