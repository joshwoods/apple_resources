

- Network Extension
-  DNS settings 

API Collection

# DNS settings

Create and manage a system-wide DNS configuration that uses built-in encrypted DNS protocols.

## Overview

With the DNS Settings feature in macOS and iOS, your app can create and manage a configuration that uses one of the built-in DNS protocols: DNS-over-TLS or DNS-over-HTTPS. The user must explictly enable your configuration in order to use the server you specify.

## Topics

### Essentials

Network Extensions Entitlement

The APIs an app can use to customize networking features.

### DNS configuration

class NEDNSSettingsManager

An object you use to create and manage a DNS settings configuration.

class NEDNSOverHTTPSSettings

The DNS resolver settings for a DNS-over-HTTPS server.

class NEDNSOverTLSSettings

The DNS resolver settings for a DNS-over-TLS server.

## See Also

### DNS configurations

DNS proxy provider

Create an on-device DNS proxy using a custom protocol.

