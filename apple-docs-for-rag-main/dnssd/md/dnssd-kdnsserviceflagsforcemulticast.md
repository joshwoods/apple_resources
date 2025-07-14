

- dnssd
-  kDNSServiceFlagsForceMulticast 

Global Variable

# kDNSServiceFlagsForceMulticast

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsForceMulticast: UInt32 { get }
```

## Discussion

Flag for signifying that a query or registration should be performed exclusively via multicast DNS, even for a name in a domain (e.g. foo.apple.com.) that would normally imply unicast DNS.

