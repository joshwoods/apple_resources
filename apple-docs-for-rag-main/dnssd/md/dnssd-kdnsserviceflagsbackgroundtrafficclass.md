

- dnssd
-  kDNSServiceFlagsBackgroundTrafficClass 

Global Variable

# kDNSServiceFlagsBackgroundTrafficClass

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsBackgroundTrafficClass: UInt32 { get }
```

## Discussion

This flag is meaningful in DNSServiceBrowse, DNSServiceGetAddrInfo, DNSServiceQueryRecord, and DNSServiceResolve. When set, it uses the background traffic class for packets that service the request.

