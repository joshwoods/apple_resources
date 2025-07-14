

- Network Extension
-  DNS proxy provider 

API Collection

# DNS proxy provider

Create an on-device DNS proxy using a custom protocol.

## Overview

A DNS proxy provider is an app extension that implements DNS proxying. You should create a DNS proxy provider if you want to take responsibility for resolving all DNS queries on the system. Typically this involves forwarding the queries in a way that improves performance, reliability or security. For example, a DNS proxy provider might:

- Forward DNS queries to a well-known Internet-wide DNS server

- Talk to a DNS proxying service using DNS over HTTPS (DoH) or DNS over TLS (DoT)

- Implement a completely custom DNS proxying protocol

For detailed information about DNS proxy provider deployment options, see TN3134: Network Extension provider deployment.

## Topics

### Essentials

Network Extensions Entitlement

The APIs an app can use to customize networking features.

### Provider

class NEDNSProxyProvider

The principal class for a DNS proxy provider app extension.

class NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

### Handling flows

class NEAppProxyTCPFlow

An object for reading and writing data to and from a TCP connection being proxied by the provider.

class NEAppProxyUDPFlow

An object for reading and writing data to and from a UDP conversation being proxied by the provider.

class NEAppProxyFlow

An abstract base class shared by NEAppProxyTCPFlow and NEAppProxyUDPFlow.

### Configuration

class NEDNSProxyManager

An object to create and manage an DNS proxy provider’s configuration.

class NEDNSProxyProviderProtocol

Configuration parameters for a DNS proxy.

## See Also

### DNS configurations

DNS settings

Create and manage a system-wide DNS configuration that uses built-in encrypted DNS protocols.

