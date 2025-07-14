

- Nearby Interaction
-  Discovering peers with Multipeer Connectivity 

Article

# Discovering peers with Multipeer Connectivity

Exchange discovery tokens over the local network.

## Overview

To start an interaction session with a nearby device, an app checks for nearby peer devices. When the app finds a peer, it creates an NISession and sends the session’s discoveryToken to the peer using the network technology on which they have agreed. An app can use Multipeer Connectivity to find nearby peers and exchange discovery tokens over the local network.

For an example app that find peer devices using Multipeer Connectivity, see Implementing Interactions Between Users in Close Proximity.

### Add Bonjour Services Plist Keys

To use the local network on iOS and iPadOS 14, your app requires the NSBonjourServices key present in its `Info.plist`. The value of the key adheres to the following convention, including `.tcp` and `.udp` extensions.

```
```

In addition, the system prompts users to grant the app explicit permission to use the local network. To control the messaging of this prompt, your app can include the `NSLocalNetworkUsageDescription` key.

### Check for a Nearby Peer

To broadcast a device’s ability to communicate through Multipeer Connectivity, your app creates an MCNearbyServiceAdvertiser. The app creates an MCNearbyServiceBrowser to find other devices advertising with the same technology. When the browser finds another device, it calls browser(_:foundPeer:withDiscoveryInfo:) and invites the peer to exchange tokens by calling invitePeer(_:to:withContext:timeout:).

After the other device receives the invitation, MCNearbyServiceAdvertiser calls advertiser(_:didReceiveInvitationFromPeer:withContext:invitationHandler:), in which the apps can begin sharing their discovery tokens.

Important

This process invites any nearby device to interact, but depending on the level of security an app requires, the app can more precisely control broadcasting, invitation, and acceptance behavior. For more information, see Multipeer Connectivity.

### Exchange Discovery Tokens

To respond to the invitation, the app sends its NI session’s discoveryToken to the peer. Because Multipeer Connectivity requires serialization of the data it transmits, the app archives it first.

```
```

When the receiving peer accepts data from the Multipeer Connectivity session, the app unarchives the data to deserialize the peer’s discovery token.

```
```

## See Also

### Phone interaction

Implementing Interactions Between Users in Close Proximity

Enable devices to access relative positioning information.

class NINearbyPeerConfiguration

A configuration that enables interaction between iPhone or Apple Watch devices.

