

- dnssd
-  kDNSServiceFlagsWakeOnResolve 

Global Variable

# kDNSServiceFlagsWakeOnResolve

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsWakeOnResolve: UInt32 { get }
```

## Discussion

This flag is meaningful only in DNSServiceResolve. When set, it tries to send a magic packet to wake up the client.

