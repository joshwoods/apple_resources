

- System Configuration
-  SCNetworkConnectionPPPStatus 

Enumeration

# SCNetworkConnectionPPPStatus

The PPP-specific status of the network connection.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum SCNetworkConnectionPPPStatus
```

## Overview

This status is returned as part of the extended information for a PPP service. Note that additional status might be returned in the future. Therefore, your application should be prepared to receive an unknown value.

## Topics

### Constants

case disconnected

PPP is disconnected.

case initializing

PPP is initializing.

case connectingLink

PPP is connecting the lower connection layer (for example, the modem is dialing out).

case dialOnTraffic

PPP is waiting for networking traffic to automatically establish the connection.

case negotiatingLink

The PPP lower layer is connected and PPP is negotiating the link layer (LCP protocol).

case authenticating

PPP is authenticating to the server (PAP, CHAP, MS-CHAP, or EAP protocols).

case waitingForCallBack

PPP is waiting for the server to call back.

case negotiatingNetwork

PPP is now authenticated and negotiating the networking layer (IPCP or IPv6CP protocols).

case connected

PPP is now fully connected for at least one networking layer. Additional networking protocol might still be negotiating.

case terminating

PPP networking and link protocols are terminating.

case disconnectingLink

PPP is disconnecting the lower level (for example, the modem is hanging up).

case holdingLinkOff

PPP is disconnected and maintaining the link temporarily off.

case suspended

PPP is suspended as a result of the suspend command (for example, when a V.92 Modem is On Hold).

case waitingForRedial

PPP has found a busy server and is waiting for redial.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum SCNetworkConnectionStatus

The current status of the network connection.

Statistics Dictionary Keys

Keys associated with values in the statistics dictionary.

Selection Options Dictionary Keys

Keys used with the SCNetworkConnectionCopyUserPreferences(_:_:_:) selection options dictionary.

