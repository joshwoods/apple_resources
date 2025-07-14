

- dnssd
-  kDNSServiceFlagsShared 

Global Variable

# kDNSServiceFlagsShared

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsShared: UInt32 { get }
```

## Discussion

Flag for registering individual records on a connected DNSServiceRef. Shared indicates that there may be multiple records with this name on the network (e.g. PTR records).

