

- Network Extension
- App proxy provider
-  VPN On Demand Rules 

API Collection

# VPN On Demand Rules

Set up VPN On Demand.

## Overview

VPN On Demand allows the system to automatically start or stop a VPN connection based on various criteria. For example, you can use VPN On Demand to configure an iPhone to start a VPN connection when it’s on Wi-Fi and stop the connection when it’s on cellular. Or, you can start the VPN connection when an app tries to connect to a specific service that’s only available via VPN.

For more information, see “VPN On Demand” in Apple Platform Deployment Guide.

## Topics

### Settings

class NEOnDemandRuleConnect

A VPN On Demand rule that connects the VPN.

class NEOnDemandRuleDisconnect

A VPN On Demand rule that disconnects the VPN.

class NEOnDemandRuleIgnore

A VPN On Demand rule that doesn’t change the status of the VPN.

class NEOnDemandRuleEvaluateConnection

A VPN On Demand rule that evaluate the app’s connection to determine whether to run its action.

class NEOnDemandRule

A base class shared by all VPN On Demand rules.

## See Also

### Related Documentation

Personal VPN

Create and manage a VPN configuration that uses one of the built-in VPN protocols (IPsec or IKEv2).

Packet tunnel provider

Implement a VPN client for a packet-oriented, custom VPN protocol.

App proxy provider

Implement a VPN client for a flow-oriented, custom VPN protocol.

### VPN configuration

class NEAppProxyProviderManager

An object to create and manage the app proxy provider’s VPN configuration.

class NETunnelProviderManager

An object to create and manage the tunnel provider’s VPN configuration.

class NEVPNManager

An object to create and manage a Personal VPN configuration.

class NETunnelProviderProtocol

Configuration parameters for a VPN tunnel.

class NEAppRule

The identity of an app whose traffic is to be routed through the tunnel.

