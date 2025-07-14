

- dnssd
-  kDNSServiceFlagsAllowRemoteQuery 

Global Variable

# kDNSServiceFlagsAllowRemoteQuery

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsAllowRemoteQuery: UInt32 { get }
```

## Discussion

Flag for creating a record for which we will answer remote queries (queries from hosts more than one hop away; hosts not directly connected to the local link).

