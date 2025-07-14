

- System Configuration
- SCNetworkConnectionPPPStatus
-  SCNetworkConnectionPPPStatus.negotiatingLink 

Case

# SCNetworkConnectionPPPStatus.negotiatingLink

The PPP lower layer is connected and PPP is negotiating the link layer (LCP protocol).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case negotiatingLink
```

## See Also

### Constants

case disconnected

PPP is disconnected.

case initializing

PPP is initializing.

case connectingLink

PPP is connecting the lower connection layer (for example, the modem is dialing out).

case dialOnTraffic

PPP is waiting for networking traffic to automatically establish the connection.

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

