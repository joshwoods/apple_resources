

- Network
-  Building a custom peer-to-peer protocol 

Sample Code

# Building a custom peer-to-peer protocol

Use networking frameworks to create a custom protocol for playing a game across iOS, iPadOS, watchOS, and tvOS devices.

Download

iOS 16.0+iPadOS 16.0+tvOS 16.0+watchOS 9.0+Xcode 15.0+

## Overview

This TicTacToe sample code project creates a networked game that you can play between different devices, communicating with a custom protocol. The game offers two ways to play:

- On Apple TV, the game uses DeviceDiscoveryUI to discover nearby iOS, iPadOS, and watchOS devices. After connecting, you can use your device to play against an AI opponent on Apple TV.

- On iOS and iPadOS devices, the game uses Bonjour and TLS to establish secure connections between nearby devices. You can use this mode to play a peer-to-peer two-player game.

Note

This sample code project is associated with WWDC22 session 110339: Build device-to-device interactions with the Network framework. It’s also associated with WWDC 2020 session 10110: Support local network privacy in your app and with WWDC 2019 session 713: Advances in Networking, Part 2.

## See Also

### Network Protocols

class NWProtocolTCP

A network protocol for connections that use the Transmission Control Protocol.

class NWProtocolTLS

A network protocol for connections that use Transport Layer Security.

class NWProtocolQUIC

A network protocol for connections that use the QUIC transport protocol.

class NWProtocolUDP

A network protocol for connections that use the User Datagram Protocol.

class NWProtocolIP

A network protocol for configuring the Internet Protocol on connections.

class NWProtocolWebSocket

A network protocol for connections that use WebSocket.

class NWProtocolFramer

A customizable network protocol for defining application message parsers.

