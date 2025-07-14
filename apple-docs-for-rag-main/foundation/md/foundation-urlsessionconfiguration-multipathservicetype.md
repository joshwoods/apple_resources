

- Foundation
- URLSessionConfiguration
-  multipathServiceType 

Instance Property

# multipathServiceType

A service type that specifies the Multipath TCP connection policy for transmitting data over Wi-Fi and cellular interfaces.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var multipathServiceType: URLSessionConfiguration.MultipathServiceType { get set }
```

## Mentioned in 

Improving network reliability using Multipath TCP

## Discussion

Multipath TCP, defined by the IETF in RFC 6824, is an extension to TCP that permits multiple interfaces to transmit a single data stream. This capability allows a seamless handover from Wi-Fi to cellular, aimed at making both interfaces more efficient and improving the user experience.

The multipathServiceType property defines which policy the Multipath TCP stack uses to schedule traffic across Wi-Fi and cellular interfaces. The default value is `none`, meaning Multipath TCP is disabled. You can also select handover mode, which provides seamless handover between Wi-Fi and cellular.

Multipath TCP requires server support. Resources for Linux-based systems are available at https://mptcp.dev.

## See Also

### Supporting Multipath TCP

Improving network reliability using Multipath TCP

Use the available radios in iOS devices to improve your app’s network reliability and performance.

enum MultipathServiceType

Constants that specify the type of service that Multipath TCP uses.

Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

