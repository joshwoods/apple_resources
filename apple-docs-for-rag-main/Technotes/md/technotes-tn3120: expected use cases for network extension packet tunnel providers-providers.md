

- Technotes
-  TN3120: Expected use cases for Network Extension packet tunnel providers 

Article

# TN3120: Expected use cases for Network Extension packet tunnel providers

Learn the expected use cases for Network Extension packet tunnel providers, and about use cases that are not supported.

## Overview

NEPacketTunnelProvider is very powerful and useful on Apple platforms. It has many valid use cases such as providing users access to secure resources and securing network traffic on an insecure network. While this API is very powerful, there are certain use cases that do not line up with its intended purpose. This technote briefly explains the recommended use cases for packet tunnel providers, along with common scenarios that are unsupported.

## Recommended use cases for packet tunnel providers

Recommended use cases for a packet tunnel provider include:

- Do use a packet tunnel provider to access secure resources on an isolated network. For example, use `NEPacketTunnelProvider` to implement an iOS or macOS VPN client that tunnels network traffic through a VPN connection into a private enterprise network. This can be done by tunneling specific destination IP and DNS traffic to the isolated network.

- Do use a packet tunnel provider to secure network access while on an insecure network. For example, use `NEPacketTunnelProvider` to implement an iOS or macOS VPN client that tunnels network traffic through a public VPN service that provides access to the wider internet. Common techniques used to achieve this functionality include creating a full tunnel VPN that routes all traffic to the remote VPN server that then forwards the traffic to its final destination.

## Unsupported uses of packet tunnel providers

While there are many reasons to use a packet tunnel provider, there are also many unsupported uses of this API. If you find yourself implementing any one of the code paths below, consider using one of the suggested alternatives:

- Do not use a packet tunnel provider to implement a network content filter. Packets that are read from NEPacketTunnelFlow are meant to be sent over a tunnel connection to a remote server for injection into a remote network. They are not meant to be dropped or re-injected back into the system. Doing so is a content filter action, as supported by one of the Network Extension Content Filter APIs. On iOS, implement a connection-based content filter using NEFilterDataProvider and NEFilterControlProvider. On macOS, implement a connection-based content filter with `NEFilterDataProvider` or a packet-based content filter with NEFilterPacketProvider. On macOS, using both providers at the same time is supported.

  There are two ways to deploy a content filter on iOS. In a managed environment, use MDM to deploy a content filter to supervised devices. In an unmanaged environment, deploy your content filter as part of a Screen Time app.

- Do not use a packet tunnel provider to intercept all DNS traffic on the system.  
  For small sets of DNS traffic inside your isolated network, this is reasonable. However, trying to intercept all DNS traffic on the system can result in endless edge cases and problems during development and deployment. As an alternative use the NEDNSProxyProvider or the DNS Settings APIs. These APIs were built for handling all DNS traffic on the system.

- Do not use a packet tunnel provider to selectively claim traffic for the packet tunnel and proxy all other traffic elsewhere. Traffic that is claimed by a `NEPacketTunnelProvider` is meant to be sent through the tunnel connection and not be routed through another interface via a proxy. The recommended alternative is to implement a NETransparentProxyProvider on macOS. On iOS, consider either claiming the network traffic that is needed for your tunnel with Per-App VPN, or claiming traffic by destination IP with includedRoutes.

- Do not use a packet tunnel provider to host a network listener or proxy server.  
  There is no reasonable alternative here other than using one of the App Proxy Provider APIs. This path is simply not a recommended use case for a packet tunnel provider or any other Network Extension.

Avoiding the unsupported scenarios will save your project many edges cases and bugs during the development and deployment process.

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-03-29** Added additional links to APIs.

- **2022-03-22** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

