

- Network Extension
-  NWTCPConnectionAuthenticationDelegate Deprecated

Protocol

# NWTCPConnectionAuthenticationDelegate

A delegate protocol to customize the TLS authentication done by a connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
protocol NWTCPConnectionAuthenticationDelegate : NSObjectProtocol
```

Deprecated

Use the sec_protocol_options_t type from the Security framework instead.

## Overview

A delegate is not required for an NWTCPConnection object.

## Topics

### Delegate methods

func shouldEvaluateTrust(for: NWTCPConnection) -> Bool

Indicate that the delegate should override the default trust evaluation for the connection.

func evaluateTrust(for: NWTCPConnection, peerCertificateChain: [Any], completionHandler: (SecTrust) -> Void)

Override the default trust evaluation for the connection.

func shouldProvideIdentity(for: NWTCPConnection) -> Bool

Indicate that the delegate can provide an identity for the connection authentication.

func provideIdentity(for: NWTCPConnection, completionHandler: (SecIdentity, [Any]) -> Void)

Provide the identity and an optional certificate chain to be used for authentication.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### TCP connections

class NWTCPConnection

An object to manage a TCP connection, with or without TLS.

Deprecated

class NWTLSParameters

TLS properties for creating a connection.

Deprecated

